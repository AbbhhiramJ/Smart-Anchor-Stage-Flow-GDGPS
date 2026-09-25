# StagePilot — Smart Anchor & Stage Flow (GDGPS)

Event operations workspace for run-of-show planning, disruption review, organizer approval, and anchor/crew briefing.

## Pages
- `index.html` — overview and guided product introduction.
- `control-room.html` — disruption simulator, impact review, approval, and briefing.
- `workspace.html` — event setup, agenda editor, local event library, backup/restore, cloud save/load.
- `login.html` — dedicated Supabase sign-in, account creation, and password reset page.
- `contact.html` — builder contact and project links.

Live app: https://stagepilot-smart-anchor-gdgps.vercel.app

## Authentication
Sign-in uses the existing Supabase Auth project. Users can sign in, create accounts, request password-reset email, and return to the workspace after authentication. Account confirmation may be required. The page uses only the public anon key; RLS protects cloud event data.

## Try it
Open Control room, simulate a 20-minute keynote delay, review the impact, and approve the revised plan. Demo uses sample data; no external messages are sent.

## Features
- Event setup and editable agenda with time validation and overlap checks.
- Delay impact review with organizer approval; revised timeline and briefing.
- Anchor cue and crew briefing; CSV export, print view, JSON backup/restore.
- Optional Supabase cloud save/load for event plans.

## Scope
This release is a single-organizer cloud-enabled workspace. Team invitations, live multi-user editing, multi-person approval chains, outbound notifications, SSO, and formal operational monitoring are not implemented.
