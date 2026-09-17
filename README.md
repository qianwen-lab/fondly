# Fondly v0.9.2 — Social flow, thoughtful Review, and goals

Release: 2026-09-17. Data schema v10. The browser storage key remains `fondly.data.v1`; this update does not move records to GitHub or a server.

## Updating an existing GitHub Pages installation

1. **Before replacing files:** On the same device/browser as your existing records, open the old Fondly → Review → Settings → Data & backup → Export all JSON. Save the private JSON somewhere safe. Never put the private JSON in your public GitHub repository.
2. Unzip `fondly-v0.9.2-github.zip` on your computer. Upload the files (`index.html`, `fondly-icon.png`, `manifest.webmanifest`, optionally `README.md`) to the repository **root**, replacing the old versions. Do not upload the ZIP file itself.
3. Allow GitHub Pages to deploy. Refresh on the **same website address and browser**. If you already have the icon and manifest, replacing only `index.html` is sufficient.
4. Confirm that Circles includes “随时可以发消息的人”, then spot-check a Person, past Social, and Learning. Use the JSON import in Settings if you need to restore your backup; importing replaces local records after confirmation.

## Changes

- The unused “Family & connections (record with care)” form field and profile section are hidden. Older family/contact fields remain untouched in stored/exported records, so simply upgrading does not destroy information.
- Adds one editable Circle named “随时可以发消息的人” for existing and new users, without putting people into it automatically. A same-named circle is not duplicated on repeated imports.
- Social remains the feature name. `Planned → Mark as Done` opens Postmortem directly. Preparation is hidden when Done, available in a collapsed “Previous preparation” view. Direct Done creation also opens Postmortem.
- Planned participants default to the actual participants on Done; “Edit people” is optional for absences and new acquaintances. Explicit first-time contact markers are available there for New people goals.
- One Social, one Recap, optional person/self/Social memories, and optional relationship-change notes. No new standalone Moment is generated. Historical Moments remain linked as older notes for data preservation.
- Saving Recap returns to read-only detail; click Edit to change it. Participant names in a Social and in its edit form link to profiles, and Back preserves unsaved form entries.
- Person memories can be edited or deleted directly in People, updating the single linked Learning record. Relationship notes can be edited in People as well, with original Social source links. Closeness can be changed separately and its date and before/after state are logged.
- Postmortem can record whether a particular relationship felt closer, more distant, different, or uncertain; optionally select context such as deeper conversation or shared experience. Review → Closer connections groups only explicitly recorded observations, linking to the original Social without claiming causation.
- Goals: Spend time together, Connect with more friends (In person / All types), Reach out, Meet new people, Reconnect, plus manual custom goals. Counts depend on Done socials, actual participants, explicit outgoing/first-time markers, sent invitations, and configurable reconnect gaps. Older goal records and their old metric definitions are kept. Home shows a compact progress summary.
- Home uses a small contextual, literary thought only when relevant records exist, not a generic encouragement or an invented personal conclusion.
- Review has My month / Learnings / Closer connections. Settings is reached from the compact gear button.
- Schema v10 migration is additive, and attempts a local snapshot of pre-v10 data; manual JSON export remains the reliable backup. JSON import/export includes all records and unknown extension fields.

## Important limitations

This is still a single-device, browser-local static web app. GitHub holds the code, not personal records. Clearing site data or using another browser/device can lose local data without a JSON backup. There is no automatic phone push or cross-device synchronization. Chromium interaction tests do not fully validate physical iPhone Safari, GitHub Pages deployment, or storage under your real production address.
