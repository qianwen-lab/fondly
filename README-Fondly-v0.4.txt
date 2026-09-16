Fondly v0.4 — GitHub Pages update (2026-09-16)

BEFORE: Open your existing Fondly → Review → Backup → Export all JSON. Keep it somewhere safe. Do not upload your private JSON to GitHub.

DEPLOY: Unzip this archive. Upload index.html, fondly-icon.png, and manifest.webmanifest to the ROOT of the SAME repository on main, replacing old files. Commit. In Settings → Pages select Deploy from a branch, main, /(root). Check Actions for a NEW deployment run. Keep the same URL: https://qianwen-lab.github.io/fondly/. If you changed devices/browsers, import the JSON in the app (local data does not sync).

NEW: Best-effort no-pinch/double-tap accidental zoom and more compact responsive forms; global check-in rules by closeness under Review → Rules, personal override/off, reminder suggestions only while app open; Event planned vs confirmed participants, inline Add Person, linked moments, post-mortem; live relationship counts and event-linked insights. Event moments select only the people actually spoken with.

LIMITATIONS: Browser data is local only; there is no background phone push, cloud sync, or AI. Mobile Safari may override viewport restrictions for accessibility; test on your own iPhone. No implication that an unrecorded meeting happened. Older untyped moments and planned guests are not assumed to count as contacts or confirmed attendance. Existing v0.3 personal cadences remain personal, while former 0/no-interval settings now inherit the closeness rule; check specific profiles and use Off when needed.

DATA: Maintains localStorage key fondly.data.v1. Explicit schema migrations v1→v2→v3→v4. Existing records, IDs and unknown fields retained. First v4 save attempts to keep an original pre-v0.4 snapshot if available storage allows; exporting JSON before updating remains essential. Import replaces current local records after confirmation.
