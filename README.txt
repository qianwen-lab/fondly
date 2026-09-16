Fondly v0.6.0 — GitHub Pages deployment

1. In the current Fondly app, go to Review > Backup and Export all JSON. Keep the export private.
2. Extract this ZIP. Upload index.html, fondly-icon.png and manifest.webmanifest into the ROOT of the existing fondly GitHub repository on the published main branch. Replace old versions, then Commit. Do not upload this ZIP as-is. Do NOT upload your private JSON to GitHub.
3. Confirm Settings > Pages is configured to publish from main/(root), or check your existing deploy workflow. Wait for the NEW deployment run to succeed and refresh your existing site.
4. Use the SAME URL and browser to retain local data. The browser stores data by origin; changing addresses or clearing data can lose it. Import your private JSON through Review > Backup if needed.

Version: v0.6.0, 2026-09-16; data schema: v6. Upgrades schemas v1–v5 using ID-preserving migrations and a best-effort pre-upgrade local snapshot; export remains necessary. No cloud sync or background push notifications.
