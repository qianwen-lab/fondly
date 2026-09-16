Fondly v0.2 — GitHub Pages deployment
======================================

FILES TO UPLOAD TO THE EXISTING fondly REPOSITORY (ROOT OF MAIN BRANCH):
- index.html             The complete working app
- fondly-icon.png        App icon / iPhone home-screen icon
- manifest.webmanifest   Home-screen web app metadata

Do not upload a personal JSON backup to a public GitHub repository.

IMPORTANT: BEFORE UPDATING
1. On your CURRENT Fondly site, open Data & backup and export a JSON backup.
2. Keep that backup somewhere safe and private.
3. Upload the three files above, overwriting the old index.html. Keep the
   SAME GitHub Pages repository, path and URL to retain browser-local data.
4. Reload the same URL. If your original data is at a different URL, import
   its backup from Review > Data & backup in the new version.

WHAT'S NEW
- Compact layout, app icon and persistent five-tab bottom navigation.
- Home: 200 original daily encouragements, upcoming socials and reminders.
- People: multiple circles, closeness and relationship intentions.
- Log: meeting type, private feelings, reflection and a new learning note.
- Circles: saved circles and one-off social-event prep lists.
- Review: monthly factual record summary, goals, learning library, and
  monthly review form with a 'Draft from my notes' button.
- Backup is now under Review > Data & backup, not in the top header.

REMINDERS
Reminders appear inside Home WHEN YOU OPEN THE APP. There are currently
NO background or push alerts, messages, calendar integration, cloud backup,
accounts or device-to-device sync. An event prep list appears under Upcoming
socials when its date has not passed. A follow-up needs a date to show in
Home's due list; undated reminders can be seen using 'View all reminders'.

GOAL COUNTS
Distinct people met: only moments marked 'In person' or 'Event / gathering'.
Distinct people contacted: only moments marked 'Call' or 'Message'.
Follow-ups: reminders marked done AFTER v0.2 logs a completion timestamp.
Custom goals: update their progress yourself. Unclassified v0.1 moments are
NOT presumed to be meetings; edit the moment and select its type if wanted.

DATA COMPATIBILITY
The localStorage key is unchanged: fondly.data.v1. The JSON schema advances
from 1 to 2. The migration preserves original record IDs and original fields;
new fields and collections are additive. On the first save of existing v1
storage, the app tries to keep a separate pre-v0.2 snapshot in localStorage
('fondly.pre-v2.backup'), exportable from Review > Data & backup. This is an
extra safeguard, NOT a substitute for a manually exported JSON backup.

Privacy reminder: Site code in a public repository is public. Friend details
remain in your current browser unless you explicitly export/share them, but
browser storage can be erased. Avoid storing unnecessary sensitive details.
