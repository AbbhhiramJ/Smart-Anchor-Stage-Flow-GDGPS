# StagePilot — Smart Anchor & Stage Flow (GDGPS)

Event operations workspace for run-of-show planning, disruption review, organizer approval, and anchor/crew briefing.

Live: https://stagepilot-smart-anchor-gdgps.vercel.app

## Sign in and cloud sync
Use the `Sign in & sync` link in the top navigation. Create an account with an accessible email address and a password of at least 12 characters. Confirm your email if prompted, then sign in. Save an event to cloud; choose it from Cloud events and open it on another device.

## Features
- Event setup, editable agenda, add/remove sessions, time validation and overlap checks.
- Delay impact review and approval; session durations preserved and revised event end shown.
- Anchor cue and crew briefing; CSV export, print view, JSON backup/restore.
- Supabase email/password authentication and cloud save/load for event plans and agenda.
- Postgres RLS policies, owner-scoped access, membership-role schema, activity records.

## Security and limits
The browser contains only the Supabase public anon key; privileged service-role keys are not included. RLS protects event data. Password minimum is 12 characters; unverified email sign-ins are disabled. Breached-password screening is not enabled because Supabase requires a paid plan for it.

This is a cloud-enabled single-organizer release, not a complete enterprise collaboration suite. Team invitation/role management UI, real-time shared editing, multi-person approval chains, automated notifications, SSO, and formal operational monitoring are not implemented.
