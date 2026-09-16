Fondly v0.3 · GitHub Pages

1. FIRST open your current Fondly → Review → Data & backup → Export all JSON. Keep that file safe.
2. Upload index.html, fondly-icon.png and manifest.webmanifest to your existing fondly repository on main, in the root folder. Commit changes.
3. Keep using EXACTLY the same https://qianwen-lab.github.io/fondly/ address and browser to retain local data. Refresh after the new deploy finishes.
4. If your repository Pages uses Deploy from a branch, set main / (root). The Actions run for the NEW commit must complete. Do not delete the repository or clear browser data.
5. Check your people and moments are intact; export a new v0.3 backup. If upgrading on another browser/device, IMPORT the exported JSON; local storage does not sync.

What changed: quote only at top; responsive mobile/date inputs; search-first multi-person picker with circle filter and quick-add; event→log preselection; optional per-person check-in cadence suggestions shown when app is open; optional explicit closeness/intention change history linked to moments; monthly Review change summary.

Reminders: manually dated reminders and opt-in cadence suggestions appear in Home when Fondly is opened. There are NO push notifications when the app/browser is closed, NO email, NO cloud sync, NO AI. Daily quote still uses a library of 200 distinct lines.

Data: same localStorage key fondly.data.v1. Schema v1 → v2 → v3 migration, preserving records and IDs. Optional local pre-v0.2 and pre-v0.3 snapshots if there is enough browser storage; JSON export is the reliable backup. Importing replaces local data after confirmation.
