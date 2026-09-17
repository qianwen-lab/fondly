# Fondly v0.9.1 — Social-first memories

Release: 2026-09-17. A small, local-only update to v0.9; **data schema remains 9**.

## Install / update

1. Open the old Fondly on the browser where your data lives. Review → Settings → Data & backup → **Export all JSON**. Keep the private JSON off your public GitHub repository.
2. Unzip and upload `index.html`, `fondly-icon.png`, and `manifest.webmanifest` to your existing GitHub Pages repository root. Replace previous files, **not** the site's URL. Do not upload the ZIP or your private JSON.
3. Wait for Pages to deploy; refresh on the **same device and browser**. You can update with only `index.html` if your icon and manifest are already there.

## Changes

- Removed **Contact (phone/email)** from People forms, People profiles, and search. Previously entered contact strings remain in existing JSON backups and records, so app upgrades do not silently destroy data; they are no longer displayed or edited in Fondly.
- People profiles have a single **Notes & remember** area. Existing notes remain. New social-derived person memories appear there automatically, with a link back to their Social. They are **entered from the Social**, not by visiting each Person to create them.
- Social details show each participant as a clickable name (view Person and Back returns to Social) plus **+ Remember** beside their name. This opens an inline form with that person preselected. The Social also has **+ Remember**, where you can choose one of its participants, **About this social**, or **About me**.
- Saving creates one linked memory in `learnings`, *not* a new Social/Moment and not a second copy of a person's note. Notes about a participant are visible on that Person automatically; notes about yourself appear in Review → Learnings; all remain linked to the originating Social. A Social with multiple participants can hold separate notes for each person. Legacy orphaned memories can still be edited in People if they have no available Social source.
- Recap's old “Worth remembering” field is now labeled **Other details about this social** so that Social-wide recap is distinct from Person/self learning. Existing text is preserved unchanged.
- No schema migration needed: remains schema v9, previous IDs, events, moments, invitations, social records and learnings preserved. Storage key remains `fondly.data.v1`.

## Verified (Chromium automated tests)

- Create/edit People with no contact UI; preserve old contact field on save without showing it.
- Plan/log a Social with two people, save with no new Moment; record different memories for each person and one About-me learning, verify IDs and ownership; Social → Person → Back and Person source link.
- Learning saved from Social appears in Review and in the right Person; no duplicate record; five bottom tabs fit 320px and 375px without horizontal overflow.
- Regression from v0.8 test data: migration keeps two old Moment notes, Socials, source IDs, unrecognized extension data, pre-v9 snapshot; remote contact not counted as in-person meetup; Circle → Person → Circle.

**Limitations:** GitHub Pages deployment, long-term persistence at your actual site origin, and physical iPhone Safari touch behavior have not been tested by these browser tests. No cross-device sync or background push notifications.
