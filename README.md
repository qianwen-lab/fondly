# Fondly v0.9.3 — faster logging, gentle memory follow-ups, safer backup

Released September 17, 2026 · data schema v11 · storage key unchanged: `fondly.data.v1`.

## Install on the existing GitHub Pages site

1. In your current Fondly, open **Review → ⚙ Settings → Data & backup → Export all JSON**. Confirm that the JSON actually downloaded and save it privately. Never upload this JSON to your public GitHub repository.
2. Unzip this package and upload `index.html`, `fondly-icon.png` and `manifest.webmanifest` to the repository root, overwriting the previous files. `README.md` is optional. Do not upload the ZIP itself.
3. Wait for GitHub Pages to deploy, then refresh the **same URL and browser**. Check a Person, a previous Social, a memory and Review. The updated Home Screen icon may require removing and adding the web app again on iPhone due to iOS icon caching; this does not require deleting browser/site data.

## What changed

- The approved icon is now the warm ivory tile with one muted pink heart, with no lettering. Applied to favicon, in-app header and iOS/manifest icon. A matching image fallback is embedded if only `index.html` gets replaced.
- Global `+` now offers **Quick log · Done**, **Plan / full Social**, Invitation and Person. Quick log asks for participants, date, type and optional name/recap. It creates exactly **one Done Social**, never a Moment; a single-person quick log launched from their profile stays on their profile. Add memories or relationship change later, only if wanted.
- Person memories have an optional **Bring this back on** date. Only explicitly dated memories appear on Home in **Worth remembering**, starting up to seven days before their date. Follow-ups offer profile, source Social, **Later** (+7 days) and **Done**; none creates a fictitious interaction. No automatic inference, push or surveillance.
- Review → Settings → Data & backup displays the time the last export was **initiated**, not a false claim that the download succeeded. Verify the downloaded JSON.
- Import now previews counts for People, Socials, Memories and Invitations, warns that it **replaces rather than merges**, and tries to save a before-import snapshot accessible via an export button. If the snapshot fails, it explicitly requires another confirmation; make a verified manual backup first.
- Additive v10→v11 migration keeps original IDs, historical notes, invitation links, Goals, status and relationship history. An optional pre-v11 snapshot is attempted on upgrade. Existing data stays on its original browser/storage key.
- Existing planned/done flow, Recap read-only/save/edit behavior, Notes & remember, type-based Goals and grounded Review remain in place.

## Limits

Local storage is still per browser and exact web origin. **There is no automatic syncing between phone and computer and no cloud backup.** The backup timestamp is only when Export was requested. Tests exercised UI flows in Chromium with a simulated storage layer because local-origin navigation was blocked in the available browser environment; this is not equivalent to testing the deployed GitHub Pages website or real iPhone Safari. Export before upgrading and verify on your device.
