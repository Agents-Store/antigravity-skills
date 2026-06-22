# google-workspace-dev (Antigravity skills)

Google Workspace plugin powered by the official googleworkspace/cli (gws) Agent Skills. ~95 skills for Gmail, Drive, Calendar, Sheets, Docs, Chat, Meet, Tasks, Slides, Forms, Classroom and Admin — plus role personas and ready-made recipes — all driving the gws CLI. Vendored from upstream and auto-synced weekly. Requires the gws CLI (npm i -g @googleworkspace/cli) and a one-time OAuth setup.

## Install

Project-scoped:
```bash
cp -r skills/* /path/to/your-project/.agent/skills/
```

User-global:
```bash
cp -r skills/* ~/.gemini/antigravity/skills/
```

## Skills (97)

- `google-workspace-dev-examples` — Use when the user wants a worked end-to-end example of combining Google Workspace services with the gws CLI — e.g. "show me an example", "how do I turn emails into tasks", "build a report from a sheet and email it", "prep for my next meeting", "create events from a spreadsheet". Walks through multi-step scenarios that chain several gws-*/recipe-* skills.
- `google-workspace-dev-google-workspace-setup` — Use when installing or troubleshooting the gws (Google Workspace CLI) that powers every google-workspace-dev skill. Triggers on "install gws", "gws auth setup", "gws auth login", "set up Google Workspace CLI", "connect Gmail/Drive/Calendar", or errors like "command not found: gws", "Access blocked", "403 accessNotConfigured", "redirect_uri_mismatch", or "too many scopes".
- `google-workspace-dev-gws-admin-reports` — Google Workspace Admin SDK: Audit logs and usage reports.
- `google-workspace-dev-gws-calendar` — Google Calendar: Manage calendars and events.
- `google-workspace-dev-gws-calendar-agenda` — Google Calendar: Show upcoming events across all calendars.
- `google-workspace-dev-gws-calendar-insert` — Google Calendar: Create a new event.
- `google-workspace-dev-gws-chat` — Google Chat: Manage Chat spaces and messages.
- `google-workspace-dev-gws-chat-send` — Google Chat: Send a message to a space.
- `google-workspace-dev-gws-classroom` — Google Classroom: Manage classes, rosters, and coursework.
- `google-workspace-dev-gws-docs` — Read and write Google Docs.
- `google-workspace-dev-gws-docs-write` — Google Docs: Append text to a document.
- `google-workspace-dev-gws-drive` — Google Drive: Manage files, folders, and shared drives.
- `google-workspace-dev-gws-drive-upload` — Google Drive: Upload a file with automatic metadata.
- `google-workspace-dev-gws-events` — Subscribe to Google Workspace events.
- `google-workspace-dev-gws-events-renew` — Google Workspace Events: Renew/reactivate Workspace Events subscriptions.
- `google-workspace-dev-gws-events-subscribe` — Google Workspace Events: Subscribe to Workspace events and stream them as NDJSON.
- `google-workspace-dev-gws-forms` — Read and write Google Forms.
- `google-workspace-dev-gws-gmail` — Gmail: Send, read, and manage email.
- `google-workspace-dev-gws-gmail-forward` — Gmail: Forward a message to new recipients.
- `google-workspace-dev-gws-gmail-read` — Gmail: Read a message and extract its body or headers.
- `google-workspace-dev-gws-gmail-reply` — Gmail: Reply to a message (handles threading automatically).
- `google-workspace-dev-gws-gmail-reply-all` — Gmail: Reply-all to a message (handles threading automatically).
- `google-workspace-dev-gws-gmail-send` — Gmail: Send an email.
- `google-workspace-dev-gws-gmail-triage` — Gmail: Show unread inbox summary (sender, subject, date).
- `google-workspace-dev-gws-gmail-watch` — Gmail: Watch for new emails and stream them as NDJSON.
- `google-workspace-dev-gws-keep` — Manage Google Keep notes.
- `google-workspace-dev-gws-meet` — Manage Google Meet conferences.
- `google-workspace-dev-gws-modelarmor` — Google Model Armor: Filter user-generated content for safety.
- `google-workspace-dev-gws-modelarmor-create-template` — Google Model Armor: Create a new Model Armor template.
- `google-workspace-dev-gws-modelarmor-sanitize-prompt` — Google Model Armor: Sanitize a user prompt through a Model Armor template.
- `google-workspace-dev-gws-modelarmor-sanitize-response` — Google Model Armor: Sanitize a model response through a Model Armor template.
- `google-workspace-dev-gws-people` — Google People: Manage contacts and profiles.
- `google-workspace-dev-gws-script` — Manage Google Apps Script projects.
- `google-workspace-dev-gws-script-push` — Google Apps Script: Upload local files to an Apps Script project.
- `google-workspace-dev-gws-shared` — gws CLI: Shared patterns for authentication, global flags, and output formatting.
- `google-workspace-dev-gws-sheets` — Google Sheets: Read and write spreadsheets.
- `google-workspace-dev-gws-sheets-append` — Google Sheets: Append a row to a spreadsheet.
- `google-workspace-dev-gws-sheets-read` — Google Sheets: Read values from a spreadsheet.
- `google-workspace-dev-gws-slides` — Google Slides: Read and write presentations.
- `google-workspace-dev-gws-tasks` — Google Tasks: Manage task lists and tasks.
- `google-workspace-dev-gws-workflow` — Google Workflow: Cross-service productivity workflows.
- `google-workspace-dev-gws-workflow-email-to-task` — Google Workflow: Convert a Gmail message into a Google Tasks entry.
- `google-workspace-dev-gws-workflow-file-announce` — Google Workflow: Announce a Drive file in a Chat space.
- `google-workspace-dev-gws-workflow-meeting-prep` — Google Workflow: Prepare for your next meeting: agenda, attendees, and linked docs.
- `google-workspace-dev-gws-workflow-standup-report` — Google Workflow: Today's meetings + open tasks as a standup summary.
- `google-workspace-dev-gws-workflow-weekly-digest` — Google Workflow: Weekly summary: this week's meetings + unread email count.
- `google-workspace-dev-persona-content-creator` — Create, organize, and distribute content across Workspace.
- `google-workspace-dev-persona-customer-support` — Manage customer support — track tickets, respond, escalate issues.
- `google-workspace-dev-persona-event-coordinator` — Plan and manage events — scheduling, invitations, and logistics.
- `google-workspace-dev-persona-exec-assistant` — Manage an executive's schedule, inbox, and communications.
- `google-workspace-dev-persona-hr-coordinator` — Handle HR workflows — onboarding, announcements, and employee comms.
- `google-workspace-dev-persona-it-admin` — Administer IT — monitor security and configure Workspace.
- `google-workspace-dev-persona-project-manager` — Coordinate projects — track tasks, schedule meetings, and share docs.
- `google-workspace-dev-persona-researcher` — Organize research — manage references, notes, and collaboration.
- `google-workspace-dev-persona-sales-ops` — Manage sales workflows — track deals, schedule calls, client comms.
- `google-workspace-dev-persona-team-lead` — Lead a team — run standups, coordinate tasks, and communicate.
- `google-workspace-dev-recipe-backup-sheet-as-csv` — Export a Google Sheets spreadsheet as a CSV file for local backup or processing.
- `google-workspace-dev-recipe-batch-invite-to-event` — Add a list of attendees to an existing Google Calendar event and send notifications.
- `google-workspace-dev-recipe-block-focus-time` — Create recurring focus time blocks on Google Calendar to protect deep work hours.
- `google-workspace-dev-recipe-bulk-download-folder` — List and download all files from a Google Drive folder.
- `google-workspace-dev-recipe-collect-form-responses` — Retrieve and review responses from a Google Form.
- `google-workspace-dev-recipe-compare-sheet-tabs` — Read data from two tabs in a Google Sheet to compare and identify differences.
- `google-workspace-dev-recipe-copy-sheet-for-new-month` — Duplicate a Google Sheets template tab for a new month of tracking.
- `google-workspace-dev-recipe-create-classroom-course` — Create a Google Classroom course and invite students.
- `google-workspace-dev-recipe-create-doc-from-template` — Copy a Google Docs template, fill in content, and share with collaborators.
- `google-workspace-dev-recipe-create-events-from-sheet` — Read event data from a Google Sheets spreadsheet and create Google Calendar entries for each row.
- `google-workspace-dev-recipe-create-expense-tracker` — Set up a Google Sheets spreadsheet for tracking expenses with headers and initial entries.
- `google-workspace-dev-recipe-create-feedback-form` — Create a Google Form for feedback and share it via Gmail.
- `google-workspace-dev-recipe-create-gmail-filter` — Create a Gmail filter to automatically label, star, or categorize incoming messages.
- `google-workspace-dev-recipe-create-meet-space` — Create a Google Meet meeting space and share the join link.
- `google-workspace-dev-recipe-create-presentation` — Create a new Google Slides presentation and add initial slides.
- `google-workspace-dev-recipe-create-shared-drive` — Create a Google Shared Drive and add members with appropriate roles.
- `google-workspace-dev-recipe-create-task-list` — Set up a new Google Tasks list with initial tasks.
- `google-workspace-dev-recipe-create-vacation-responder` — Enable a Gmail out-of-office auto-reply with a custom message and date range.
- `google-workspace-dev-recipe-draft-email-from-doc` — Read content from a Google Doc and use it as the body of a Gmail message.
- `google-workspace-dev-recipe-email-drive-link` — Share a Google Drive file and email the link with a message to recipients.
- `google-workspace-dev-recipe-find-free-time` — Query Google Calendar free/busy status for multiple users to find a meeting slot.
- `google-workspace-dev-recipe-find-large-files` — Identify large Google Drive files consuming storage quota.
- `google-workspace-dev-recipe-forward-labeled-emails` — Find Gmail messages with a specific label and forward them to another address.
- `google-workspace-dev-recipe-generate-report-from-sheet` — Read data from a Google Sheet and create a formatted Google Docs report.
- `google-workspace-dev-recipe-label-and-archive-emails` — Apply Gmail labels to matching messages and archive them to keep your inbox clean.
- `google-workspace-dev-recipe-log-deal-update` — Append a deal status update to a Google Sheets sales tracking spreadsheet.
- `google-workspace-dev-recipe-organize-drive-folder` — Create a Google Drive folder structure and move files into the right locations.
- `google-workspace-dev-recipe-plan-weekly-schedule` — Review your Google Calendar week, identify gaps, and add events to fill them.
- `google-workspace-dev-recipe-post-mortem-setup` — Create a Google Docs post-mortem, schedule a Google Calendar review, and notify via Chat.
- `google-workspace-dev-recipe-reschedule-meeting` — Move a Google Calendar event to a new time and automatically notify all attendees.
- `google-workspace-dev-recipe-review-meet-participants` — Review who attended a Google Meet conference and for how long.
- `google-workspace-dev-recipe-review-overdue-tasks` — Find Google Tasks that are past due and need attention.
- `google-workspace-dev-recipe-save-email-attachments` — Find Gmail messages with attachments and save them to a Google Drive folder.
- `google-workspace-dev-recipe-save-email-to-doc` — Save a Gmail message body into a Google Doc for archival or reference.
- `google-workspace-dev-recipe-schedule-recurring-event` — Create a recurring Google Calendar event with attendees.
- `google-workspace-dev-recipe-send-team-announcement` — Send a team announcement via both Gmail and a Google Chat space.
- `google-workspace-dev-recipe-share-doc-and-notify` — Share a Google Docs document with edit access and email collaborators the link.
- `google-workspace-dev-recipe-share-event-materials` — Share Google Drive files with all attendees of a Google Calendar event.
- `google-workspace-dev-recipe-share-folder-with-team` — Share a Google Drive folder and all its contents with a list of collaborators.
- `google-workspace-dev-recipe-sync-contacts-to-sheet` — Export Google Contacts directory to a Google Sheets spreadsheet.
- `google-workspace-dev-recipe-watch-drive-changes` — Subscribe to change notifications on a Google Drive file or folder.

## Source

Canonical: https://github.com/agents-store/claude-public-plugins/tree/main/plugins/google-workspace-dev
