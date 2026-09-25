# StagePilot — Smart Anchor & Stage Flow (GDGPS)

Event operations workspace for run-of-show planning, disruption review, organizer approval, and anchor/crew briefing.

## Live app
https://stagepilot-smart-anchor-gdgps.vercel.app

## Features
- Event setup, editable agenda, add/remove sessions, time validation and overlap checks.
- Delay impact review and approval; session durations are preserved and the revised end time is surfaced.
- Anchor cue and crew briefing; CSV export, print view, JSON backup/restore.
- Supabase email/password authentication and cloud save/load for event plans and agenda.
- Postgres RLS policies, owner-scoped access, membership-role schema, and activity records.

## Security and limitations
The browser contains only the Supabase public anon key; privileged service-role keys are not included. RLS protects event data. Password minimum is 12 characters; unverified email sign-ins are disabled. Breached-password screening is not enabled because Supabase requires a paid plan for that feature.

This is a cloud-enabled single-organizer release, not a complete enterprise collaboration suite. Team invitation/role-management UI, real-time shared editing, multi-person approval workflows, automated email/SMS/WhatsApp notifications, calendar/venue integrations, SSO, and formal operational monitoring are not yet implemented. Membership roles exist in the schema but are not yet manageable through the app.

Email confirmation is enabled. Create an account with an accessible email address, confirm it if prompted, then sign in.

## Database
Supabase project `hmpilxqzsnfjzqdeuwtd`, Mumbai region. SQL migration: `supabase/migrations/202609250820_stagepilot_core.sql`.

## Local run
Open `index.html` in a modern browser. Cloud features need internet access.

## Contact
Abbhhiram Jadhav · https://Abbhhi.dev · abbhhiram25@gmail.com
