Fondly v0.7 · September 17, 2026

Upload index.html, fondly-icon.png, and manifest.webmanifest from this archive into the ROOT of the SAME GitHub repository. Commit on the Pages publishing branch; do NOT upload the ZIP itself or any personal JSON backup.

Before updating: open your current Fondly → Review → Backup → Export all JSON. Keep that file privately, off GitHub.

What changed:
- Clear distinction: log an ordinary conversation (coffee, run, chance encounter); create an Event only when planning or recapping a gathering. An Event may contain conversations; do not create duplicate records.
- One learning note has an explicit home: Person profile, Event, or Review → My discoveries. Old v0.6 notes are preserved and can be moved deliberately.
- Event → Person, Event → conversation, Circle → Person, and Review → linked record now return to the originating page with scroll position.
- Add existing or new people directly inside Circle; remove from Circle without deleting profiles.
- Event after-notes use plain language and an optional person-specific change note; monthly goal labels are simpler.
- Data schema 7 migrates v0.1–v0.6 backups. IDs and unknown data fields are retained. An automatic v0.6 snapshot is attempted on the first new save if browser storage permits; JSON export remains essential.

Important:
- Data still resides in localStorage under fondly.data.v1 at your exact site address. Updating index.html on the SAME Pages URL preserves browser-local records under ordinary conditions, but not across devices, browser resets or private browsing.
- Reminders appear when Fondly is open; background phone push and cloud sync are NOT included.
- The existing warm-brown f. icon remains bundled for continuity; the more detailed memory-book icon redesign is still a separate visual task.
- The archive contains code and public assets only: no friends or backup data.
