# StagePilot — Smart Anchor & Stage Flow (GDGPS)

StagePilot is a browser-based event operations workspace for building and maintaining run-of-show plans, reviewing schedule disruptions, approving changes, and preparing anchor/crew communications.

## Live app
https://stagepilot-smart-anchor-gdgps.vercel.app

## Operational features
- Manage multiple event plans in the same browser workspace.
- Configure event name, venue, date, and organizer.
- Add, edit, and remove agenda sessions and assign speakers/owners.
- Validate session time ranges and prevent overlapping sessions.
- Review a selected-session delay before approval; downstream session durations are preserved and the event end shift is shown.
- Maintain plan version, anchor cue, and crew briefing.
- Export the run of show as CSV, download a JSON event backup, restore a backup, and print the run of show.
- Persist plans in browser storage.

## Important deployment limits
This version is a single-organizer browser application. Data is stored in the current browser/device and is not shared with other organizers. It does not provide account authentication, cloud database synchronization, live multi-user collaboration, venue integrations, or automatic email/SMS/WhatsApp messaging. Use JSON backups to transfer plans. A production multi-user rollout requires a secure backend, authentication, role-based access, audit history, and server-side persistence.

## Run locally
Open `index.html` in a modern browser. No build step, install, or API key is required.

## Contact
Abbhhiram Jadhav · https://Abbhhi.dev · abbhhiram25@gmail.com
