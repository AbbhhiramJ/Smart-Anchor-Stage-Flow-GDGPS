# StagePilot — Smart Anchor & Stage Flow (GDGPS)

StagePilot is an event operations workspace that helps an organizer respond to schedule disruptions with a reviewed run-of-show, anchor cue, and crew briefing.

Live app: https://stagepilot-smart-anchor-gdgps.vercel.app

## Try the experience
1. Open the app and choose **Enter the control room**.
2. Choose **Start guided scenario**.
3. Review the proposed 20-minute keynote delay.
4. Approve the revised run of show to see the timeline, anchor cue, briefing, and activity log update.

No account is needed to try the sample scenario.

## Features
- Event setup, editable agenda, add/remove sessions, time validation and overlap checks.
- Delay impact review with organizer approval; session durations preserved and revised event end surfaced.
- Anchor cue and crew briefing; CSV export, print view, JSON backup/restore.
- Supabase email/password authentication and explicit cloud save/load for event plans and agenda.
- Postgres row-level security, owner-scoped access, membership-role schema, and activity records.

## Data and security
Browser-local workspace works without signing in. Cloud save/load is optional and requires an account. The browser contains only the Supabase public anon key; privileged service-role credentials are not shipped. Database RLS restricts event data. Password minimum is 12 characters; unverified email sign-ins are disabled.

This release is a single-organizer cloud-enabled workspace, not a complete enterprise collaboration suite. Team invitations/role management UI, real-time shared editing, multi-person approval chains, automated outbound notifications, SSO, and formal operational monitoring are not implemented.

## Contact
Abbhhiram Jadhav · https://Abbhhi.dev · abbhhiram25@gmail.com
