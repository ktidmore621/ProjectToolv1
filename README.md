# Customer Assignment Tracker

A lightweight, single-file workflow/project management tool for **Customer Assignment
Projects** — one project per MCP/client, tracked from assignment through formal closure.

Open `customer-assignment-tracker.html` in a browser. No server, no build step —
all data is stored in the browser's localStorage (existing v1 data is migrated
automatically).

## Modules

- **Dashboard** — active projects, overdue/blocked tasks, time logged, projects by
  status and RAG, open work by assignee, time by user, closures per month, aging.
- **Projects** — create from a workflow template (one active project per MCP is
  enforced), search/filter, project detail with status, risk level, and
  auto-calculated RAG with manual override.
- **Tasks** — generated from the selected template; template tasks cannot be deleted
  or reordered, required tasks can only be skipped with a reason, ad-hoc tasks can
  be added freely. Due dates, priorities, and completion tracking.
- **Time logging** — hours/minutes per task with activity types; rolls up to task
  and project; users edit/delete their own logs (admins any), all recorded in
  activity history.
- **Notes & activity** — categorized rich-text notes at project and task level;
  status changes, time logs, and overrides are auto-captured in history.
- **Closure & history** — closing requires all required tasks Complete/Skipped
  (admin override available), a close reason, and a final summary. Closed and
  cancelled projects are permanent, read-only records in the History view; a new
  assignment for the same MCP means a new project.
- **Template admin** (Admin role) — create/edit workflow templates, task order,
  required flags, priorities, due-date offsets; mark one template as default;
  activate/deactivate.

## Roles

Set your name and role (User/Admin) in the header. Admins manage templates and may
override closure requirements.
