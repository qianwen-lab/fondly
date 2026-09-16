FONDLY v0.5 — GitHub Pages release
==================================

Files to deploy (upload all three to the repository ROOT):
- index.html
- fondly-icon.png
- manifest.webmanifest

WHAT CHANGED
- People: six sorting options, separate circle / closeness / intention / activity filters, search, clear filters, and persistent filter/sort preferences (stored only in the same browser).
- Invitations: track person, date, response, notes, optional revisit date, own next step and learning. Access from Log -> + Invite or a person's profile. Outcome labels: awaiting reply / accepted / unavailable / declined / rescheduled.
- Accepted invitation -> create linked Event, with that person preselected. The invitation remains independent in the person's timeline.
- Events: one + Event entry in Circles (no separate Plan button); single Event entity holds planned people, actual attendance, related moments and post-mortem. Event statuses: planned / completed / cancelled.
- Solo activities are out of scope. Invitation is not a meeting and does not automatically reset check-in or change closeness.
- Home shows invitation follow-ups if explicitly set to Try again later with a revisit date. Review shows invitation outcome counts and your optional learnings.
- All pre-existing v0.4 responsive/mobile zoom mitigations, 5 bottom tabs, rules, reflection, icons, and export/import remain.

UPDATE YOUR EXISTING SITE
1. FIRST open the current Fondly -> Review -> Backup -> Export all JSON.
2. Unzip this ZIP. Upload/replace index.html, fondly-icon.png, manifest.webmanifest in the SAME repo and root directory, and commit to main. Do not upload the ZIP itself or upload this README unless desired.
3. In GitHub Settings -> Pages choose Deploy from a branch, main, /(root). Check Actions for a NEW deployment of the latest commit. Wait for it to succeed; if an old version shows, reload the exact same Pages address.
4. Stay on the same GitHub Pages URL and browser. Your localStorage belongs to that exact address and browser; a new URL or device does NOT automatically have your data. Import your exported JSON if needed.

DATA SAFETY
- Storage key remains fondly.data.v1, data schema upgraded to v5. Migrations for v1, v2, v3 and v4 preserve IDs and unknown fields. First upgrade save attempts to preserve pre-v5 raw storage under fondly.pre-v5.backup, if browser capacity allows. Export JSON is the reliable backup.
- Import replaces current records only after confirmation. Export before importing.
- Data is browser-local; not stored by GitHub in repository, and not synced. No background push notifications. Due check-ins and invitations are shown only when Fondly is opened.
- Date / contact / invitation insights come from user-entered records. No assumptions about why another person declines, or automatic relationship scoring.
- Only commit app files, NEVER your private JSON backup, to a public repo.
