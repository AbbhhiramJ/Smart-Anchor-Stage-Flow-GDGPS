# StagePilot — Smart Anchor & Stage Flow (GDGPS)

StagePilot is an event operations workspace for reviewing schedule disruptions, approving run-of-show changes, and preparing anchor/crew communications.

## Pages
- **Overview:** `index.html` — product introduction and guided experience entry.
- **Control room:** `control-room.html` — disruption simulator, impact review, approval, and updated briefing.
- **Event workspace:** `workspace.html` — event setup, agenda editor, plan library, backups, and cloud sign-in/sync.
- **Contact:** `contact.html` — builder contact and project/source links.

Live app: https://stagepilot-smart-anchor-gdgps.vercel.app

## Try it
Open Control room, simulate a 20-minute keynote delay, review the impact, and approve the revised plan. Sample demo data is used; no external messages are sent.

## Features
- Event setup and editable agenda with time validation and overlap checks.
- Delay impact review with organizer approval; revised timeline and briefing.
- Anchor cue and crew briefing; CSV export, print view, JSON backup/restore.
- Supabase email/password authentication and explicit cloud save/load.
- Postgres row-level security, owner-scoped access, membership-role schema, activity records.

## Security and scope
The browser uses only the Supabase public anon key; privileged service-role credentials are not shipped. RLS restricts event data. Password minimum is 12 characters; unverified email sign-ins are disabled. This release is a single-organizer cloud-enabled workspace; team invitation UI, live multi-user editing, multi-person approval chains, outbound notifications, SSO, and formal operational monitoring are not implemented.
