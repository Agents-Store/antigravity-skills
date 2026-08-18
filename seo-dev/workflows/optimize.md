# optimize

Full SEO optimization — audit, fix, and enhance SEO across Next.js and Directus

Arguments: [--skip-directus] [--skip-build] [--report-only]

# SEO Optimize

End-to-end SEO optimization for a Directus + Next.js project. Audits the current state, implements all fixes, extends Directus schema with SEO fields, and produces a final report.

## Arguments

- `--skip-directus` (optional) — Skip Directus schema changes and field population
- `--skip-build` (optional) — Skip the final `pnpm build` verification
- `--report-only` (optional) — Audit only, do not make changes. Show what needs fixing

## Skills Used

This command orchestrates all seo-dev skills plus Directus MCP tools:

| Skill | Used In |
|-------|---------|
| `seo-dev:setup` | Phase 1: Audit foundations |
| `seo-dev:meta-tags` | Phase 2: Metadata & OG |
| `seo-dev:structured-data` | Phase 3: JSON-LD |
| `seo-dev:sitemap-robots` | Phase 4: Sitemap & Robots |
| `seo-dev:performance` | Phase 5: Core Web Vitals |
| `seo-dev:technical-seo` | Phase 6: Technical SEO |
| `seo-dev:content-seo` | Phase 7: Content optimization |
| `seo-dev:audit` | Phase 1 & Phase 8: Audit & Report |
| `directus-dev:schema-design` | Phase 1g: Schema audit |
| `directus-dev:mcp-tools` | Phase 3D: Field creation & item population |
| `stack-directus-nextjs-dev:directus-to-nextjs` | Phase 3D-4: Data fetching updates |

## Process

### Phase 1: SEO Audit (read-only)

Scan the entire project to understand the current SEO state. Do NOT make changes yet — collect findings first.

#### 1a. Project Structure Discovery

```bash
# Find the app directory
ls -d src/app 2>/dev/null || ls -d app 2>/dev/null

# Identify all page routes
find src/app -name "page.tsx" -o -name "page.ts" 2>/dev/null || find app -name "page.tsx" -o -name "page.ts" 2>/dev/null

# Find root layout
find src/app -name "layout.tsx" -maxdepth 1 2>/dev/null || find app -name "layout.tsx" -maxdepth 1 2>/dev/null
```

#### 1b. Metadata Audit

Check every page and layout for metadata:

```bash
# Pages with metadata
grep -rl "export const metadata\|export async function generateMetadata" src/app --include="*.tsx" --include="*.ts"

# Pages WITHOUT metadata (these need fixing)
find src/app -name "page.tsx" | while read f; do
  grep -qE "metadata|generateMetadata" "$f" || echo "MISSING: $f"
done

# Check metadataBase
grep -r "metadataBase" src/app/layout.tsx

# Check title template
grep -r "template:" src/app/layout.tsx

# Check NEXT_PUBLIC_SITE_URL
grep "NEXT_PUBLIC_SITE_URL" .env .env.local 2>/dev/null
```

#### 1c. Sitemap & Robots Audit

```bash
ls src/app/sitemap.ts src/app/robots.ts 2>/dev/null
```

#### 1d. Structured Data Audit

```bash
# Check for existing JSON-LD
grep -rl "application/ld+json" src/ --include="*.tsx" --include="*.ts"

# Check for schema-dts
grep "schema-dts" package.json

# Check for JsonLd component
grep -rl "JsonLd" src/components/ --include="*.tsx" 2>/dev/null
```

#### 1e. Images Audit

```bash
# Images without alt text
grep -rn "<Image\|<img" src/ --include="*.tsx" | grep -v "alt=" | head -30

# Images without sizes prop
grep -rn "<Image" src/ --include="*.tsx" | grep -v "sizes=" | head -20

# Images with priority prop (should be only LCP images)
grep -rn "priority" src/ --include="*.tsx" | grep "<Image\|Image " | head -10

# Check next.config for image formats
grep -A5 "images:" next.config.ts 2>/dev/null || grep -A5 "images:" next.config.js 2>/dev/null
```

#### 1f. Heading Hierarchy Audit

```bash
# Count H1 tags per page
find src/app -name "page.tsx" | while read f; do
  count=$(grep -c "<h1\|<H1" "$f" 2>/dev/null || echo "0")
  [ "$count" != "1" ] && echo "H1 count=$count: $f"
done
```

#### 1g. Directus Schema Audit (skip if --skip-directus)

Use Directus MCP tools to discover content collections and check for SEO fields.

**Step 1: Discover all collections**

Call the `schema` tool with no parameters to get the full collection list:

```
Tool: schema
Input: {}
```

**Step 2: Identify content collections**

From the schema response, identify content collections — those that have a `slug` or `name`/`title` field and represent public-facing content (e.g., `components`, `posts`, `pages`, `products`). Skip system collections and junction tables.

**Step 3: Get detailed schema for each content collection**

```
Tool: schema
Input: { "keys": ["components", "posts"] }
```

**Step 4: Check for SEO fields**

For each content collection, check if these fields exist:
- `meta_title` (string) — SEO title override
- `meta_description` (text) — SEO description override
- `og_image_url` (string) — Open Graph image URL
- `canonical_url` (string) — Custom canonical URL

Record which collections need SEO fields added vs. which already have them.

#### 1h. Compile Audit Report

Present findings in this format before proceeding:

```
## SEO Audit Results

### Foundations
- [ ] metadataBase: [present/missing]
- [ ] Title template: [present/missing]
- [ ] NEXT_PUBLIC_SITE_URL: [present/missing]
- [ ] sitemap.ts: [present/missing]
- [ ] robots.ts: [present/missing]
- [ ] schema-dts: [installed/missing]

### Pages (X total)
- Pages with metadata: X/Y
- Pages without metadata: [list]
- Pages missing canonical: [list]

### Structured Data
- JSON-LD present: [yes/no]
- Organization schema: [yes/no]
- WebSite schema: [yes/no]
- Page-specific schemas: [list]

### Images
- Images without alt: X
- Images without sizes: X
- LCP images without priority: X

### Headings
- Pages with wrong H1 count: [list]

### Directus SEO Fields
- Content collections found: [list]
- Collections with all 4 SEO fields (meta_title, meta_description, og_image_url, canonical_url): [list]
- Collections missing SEO fields: [list with which fields are missing]
- Items with empty meta_title: X/Y total

### Estimated changes: X files to create/modify
```

**If --report-only**: stop here, show the report, and exit.

Ask the user to confirm before proceeding with changes.

### Phase 2: SEO Foundations

Apply `seo-dev:setup` patterns.

#### 2a. Install schema-dts

```bash
pnpm add -D schema-dts
```

#### 2b. Set NEXT_PUBLIC_SITE_URL

If missing from `.env` / `.env.local`, add it:
```
NEXT_PUBLIC_SITE_URL=https://yourdomain.com
```

Ask the user for their production domain if not already set.

#### 2c. Configure Root Layout Metadata

Read the current root layout. Add or update:

```tsx
import type { Metadata } from 'next'

export const metadata: Metadata = {
  metadataBase: new URL(process.env.NEXT_PUBLIC_SITE_URL || 'http://localhost:3000'),
  title: {
    template: '%s | Site Name',
    default: 'Site Name',
  },
  description: 'Site description',
  openGraph: {
    type: 'website',
    siteName: 'Site Name',
    locale: 'en_US',
  },
  twitter: {
    card: 'summary_large_image',
  },
}
```

Preserve any existing metadata fields. Merge, do not replace.

#### 2d. Create robots.ts (if missing)

Apply `seo-dev:sitemap-robots` pattern with environment-aware blocking and AI crawler rules.

#### 2e. Create sitemap.ts (if missing)

Apply `seo-dev:sitemap-robots` dynamic pattern. Fetch pages from Directus:

```tsx
import type { MetadataRoute } from 'next'
import directus from '@/lib/directus'
import { readItems } from '@directus/sdk'

const BASE_URL = process.env.NEXT_PUBLIC_SITE_URL || 'https://yourdomain.com'

export default async function sitemap(): Promise<MetadataRoute.Sitemap> {
  // Static pages
  const staticPages: MetadataRoute.Sitemap = [
    { url: BASE_URL, lastModified: new Date(), changeFrequency: 'daily', priority: 1 },
  ]

  // Dynamic pages from Directus
  // Adapt collection names and slugs to the actual project
  try {
    const posts = await directus.request(
      readItems('posts', {
        fields: ['slug', 'date_updated'],
        filter: { status: { _eq: 'published' } },
      })
    )

    const postEntries: MetadataRoute.Sitemap = posts.map((post) => ({
      url: `${BASE_URL}/blog/${post.slug}`,
      lastModified: post.date_updated ? new Date(post.date_updated) : new Date(),
      changeFrequency: 'weekly' as const,
      priority: 0.7,
    }))

    return [...staticPages, ...postEntries]
  } catch {
    return staticPages
  }
}
```

Adapt collection names (`posts`, `pages`, `products`) to match the actual project schema discovered in Phase 1.

### Phase 3: Structured Data

Apply `seo-dev:structured-data` patterns.

#### 3a. Create JsonLd Component

```tsx
// components/json-ld.tsx
import type { Thing, WithContext } from 'schema-dts'

export function JsonLd<T extends Thing>({ data }: { data: WithContext<T> }) {
  return (
    <script
      type="application/ld+json"
      dangerouslySetInnerHTML={{
        __html: JSON.stringify(data).replace(/</g, '\\u003c'),
      }}
    />
  )
}
```

#### 3b. Create Schema Factory Functions

Create `lib/schema.ts` with factory functions from the `seo-dev:structured-data` skill:
- `createOrganization`
- `createWebSite`
- `createBreadcrumbList`
- `createArticle` (if blog/news exists)
- `createProduct` (if e-commerce exists)

#### 3c. Add Sitewide Schemas to Root Layout

Add `<JsonLd>` for Organization and WebSite to the root layout `<body>`.

#### 3d. Add Page-Specific Schemas

For each content page type discovered in Phase 1:
- Blog posts → Article schema
- Product pages → Product schema
- All inner pages → BreadcrumbList schema

### Phase 3D: Directus SEO Fields (skip if --skip-directus)

**This phase is MANDATORY unless `--skip-directus` is passed.** It creates SEO fields in Directus content collections via MCP tools and auto-populates existing records. Do NOT skip this or defer it to a separate request.

#### 3D-1. Create SEO fields via MCP

For each content collection identified in Phase 1g that lacks SEO fields, call the `fields` tool to create all four fields in a single batch.

**IMPORTANT**: The `data` parameter must always be an **array** of field objects, even for a single field. Each field object must include `field`, `type`, `meta`, and `schema`.

```
Tool: fields
Input: {
  "action": "create",
  "collection": "<collection_name>",
  "data": [
    {
      "field": "meta_title",
      "type": "string",
      "meta": {
        "interface": "input",
        "display": "raw",
        "note": "SEO title for search engines (50-60 chars). Falls back to main title if empty.",
        "options": { "trim": true, "placeholder": "Override page title for search results..." },
        "width": "half",
        "sort": 100
      },
      "schema": {
        "data_type": "varchar",
        "max_length": 70,
        "is_nullable": true
      }
    },
    {
      "field": "meta_description",
      "type": "text",
      "meta": {
        "interface": "input-multiline",
        "display": "raw",
        "note": "SEO description (150-160 chars). Falls back to main description if empty.",
        "options": { "trim": true, "placeholder": "Override description for search results..." },
        "width": "full",
        "sort": 101
      },
      "schema": {
        "data_type": "text",
        "is_nullable": true
      }
    },
    {
      "field": "og_image_url",
      "type": "string",
      "meta": {
        "interface": "input",
        "display": "raw",
        "note": "Open Graph image URL (1200x630 recommended). Used for social media previews.",
        "options": { "trim": true, "placeholder": "https://..." },
        "width": "half",
        "sort": 102
      },
      "schema": {
        "data_type": "varchar",
        "max_length": 500,
        "is_nullable": true
      }
    },
    {
      "field": "canonical_url",
      "type": "string",
      "meta": {
        "interface": "input",
        "display": "raw",
        "note": "Custom canonical URL. Leave empty to use the default page URL.",
        "options": { "trim": true, "placeholder": "https://..." },
        "width": "half",
        "sort": 103
      },
      "schema": {
        "data_type": "varchar",
        "max_length": 500,
        "

<!-- truncated: content exceeds the target's size limit -->