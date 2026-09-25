# StagePilot — Smart Anchor & Stage Flow (GDGPS)

StagePilot is an event operations workspace for maintaining a run-of-show, reviewing schedule disruptions, approving changes, and preparing anchor/crew communications.

## Production workspace
https://stagepilot-smart-anchor-gdgps.vercel.app

## Current capabilities
- Configure event name, venue, date, organizer, and agenda sessions.
- Manage multiple local event plans, add/remove sessions, validate times and prevent overlaps.
- Review and approve downstream schedule shifts while preserving session durations.
- Prepare cue and crew briefing text; export CSV, print the schedule, and download/restore JSON backups.
- Create an account/sign in through Supabase Auth.
- Save and load events and agenda items in Supabase Postgres, scoped by authenticated account and database RLS.
- Record event plan changes in the activity table.

## Data and security model
- Frontend uses only the Supabase public anon key; privileged service-role credentials are not shipped to the browser.
- Postgres RLS protects events, membership, agenda items, and activity records.
- Events are owner-scoped by default. Membership roles (`owner`, `manager`, `crew`, `viewer`) are represented in the schema.
- Browser-local workspace remains available without sign-in; cloud saves are explicit.

## Current operational boundaries
This release supports authenticated cloud save/load for an individual account. It does not yet expose team invitations or a user/role management screen, real-time collaborative editing, approval chains across users, scheduled email/SMS/WhatsApp delivery, venue/calendar integrations, or a formal enterprise SSO setup. Those require additional product work and operational configuration.

Email confirmation is enabled by default. Sign up with an address you can access, confirm the email if prompted, then sign in.

## Database setup
Supabase project: `hmpilxqzsnfjzqdeuwtd` (Mumbai region). SQL migrations are stored in `supabase/migrations/`.

## Run locally
Open `index.html` in a modern browser. No build step is required. Supabase cloud features require network access.

## Contact
Abbhhiram Jadhav · https://Abbhhi.dev · abbhhiram25@gmail.com
