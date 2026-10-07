HEX FFXIV Duty Tracker - Desktop Preview v006
Application version: 0.1.5
Prepared: October 6, 2026

v006 adds offline quest tutorials below the existing information in each
expanded duty card. All 510 listed entries have instructions, including
standard quests, short NPC unlocks, raid milestones, and archived duties.

OPEN THE APP

Apple Silicon Mac (M-series): use the Mac_AppleSilicon ZIP.
Intel Mac: use the Mac_Intel ZIP.
Extract the ZIP, move HEX FFXIV Duty Tracker.app to Applications, and open it.
Requires macOS 13 Ventura or newer. No preparation command is included.
The Mac preview has an ad-hoc signature; it has no Apple Developer ID
signature or notarization, so macOS can still require app-specific approval.

Windows: extract the entire Windows ZIP and open HEX FFXIV Duty Tracker.exe.
Keep its supporting files together. Requires Windows 10 or newer on a 64-bit
Intel/AMD computer. This Windows preview is unsigned.

The app needs no ChatGPT account, email, password, or online registration.
Profiles and progress are saved locally on each computer. This release does
not create a public website or public GitHub release.

PERSONAL PROGRESS

1. Open the tracker; the default profile is My character.
2. Click the profile name to create or switch character profiles.
3. Mark duties unlocked. Each profile saves its checklist automatically.
4. Set Your level; leave the field or press Enter to save it.
5. Close and reopen the app to restore the selected profile and progress.

Profiles are local checklists. They are not password-protected online accounts.
People using the same operating-system account can open those profiles.

QUEST TUTORIALS

Expand a duty using its title or unlock-quest button. The tutorial appears
below the existing location, prerequisites, status, map, and source link.
It grows with its content; there is no separate scrolling panel or height cap.

Each tutorial gives the starting NPC, prerequisites, and ordered instructions.
An additional Access to section explains any duty-specific requirements.
The full quest can include steps after its duty unlocks; do not assume that
finishing the entire quest is required before entering its own battle.

For A Relic Reborn, Simply the Hest, A Pup No Longer, and Like Civilized Men
and Women, choose the matching job, starting city, or Grand Company. No
variant is selected automatically. These selectors cover 19 actual variants.

Instructions work offline. Quest source, Unlock source, and Duty access source
links open their wiki pages in your default browser and require internet.
Reading tutorials, changing a tutorial variant, and opening sources do not
change saved duty progress. Tutorials may reveal later quest objectives.

The source audit checked 800 retrieved wiki pages, 1,282 listed objective
facts, exact chat/emote inputs, names, quantities, prerequisites, and coverage.
This is a source-based check, not an in-game completion test. The included
quest tutorial audit describes the scope, corrections, and testing limits.

WIKI LINKS AND STATIC MAPS

The existing Wiki, Quests, and Guide links still open in your default browser.
Click a map beside the coordinates to enlarge it; close with its button or
Escape. The red marker shows the listed X/Y position.

The retained catalog has 510 entries: 495 current and 15 archived, through
patch 7.56. All 473 numerical coordinates have previews: 453 terrain maps and
20 clearly labeled coordinate guides where no terrain image was verified.
The 85 terrain images and fixed background remain included offline.

BACK UP OR MOVE PROGRESS

Export backup saves the selected profile to a JSON file you choose.
Import backup creates a new profile without overwriting existing profiles.
Backups can move between Mac and Windows. There is no automatic cloud sync.
Export a backup before changing computers or replacing your application.

Automatic save locations:
Windows: %APPDATA%\HEX FFXIV Duty Tracker\tracker-data\progress.json
Mac: ~/Library/Application Support/HEX FFXIV Duty Tracker/tracker-data/progress.json

The application name, bundle ID, duty IDs, save location, and save format are
retained from v005. Saves remain outside the application folder. Previous-save
recovery preserves damaged files and reports any failure instead of claiming
that a failed change was saved.

SOURCE AND VALIDATION

The Source ZIP contains the app source, compiled interface, curated tutorial
JSON, offline maps, source provenance, objective facts, audit results, and tests.
It excludes raw wiki HTML, player saves, credentials, and downloaded runtimes.
The included tutorial data builds without downloading wiki pages.

With Node.js 22.13 or newer, run these commands in the source folder:
npm ci
npm test
npm run typecheck
npm run build
npm start

npm run package builds Windows x64, Mac Apple Silicon, and Mac Intel bundles.
On macOS it uses codesign. Mac packaging on Linux requires rcodesign 0.29.0;
set HEX_RCODESIGN_PATH to its executable. HEX_PACKAGE_TARGET can be set to
mac or windows. Packages include README.txt beside and inside the app.

Package checks:
node scripts/verify-packages.mjs
python3 scripts/verify-mac-signatures.py

The research-only extraction, compilation, and source-audit scripts require
the separate research cache. Normal builds and the shipped regression tests
do not require it. Source provenance and factual audit evidence are included;
full wiki journal/dialogue text is not distributed.

Native macOS/Windows launch, operating-system dialogs, Gatekeeper, and antivirus
scans have not been performed in this Linux build environment. The tests use
the actual React interface, native IPC handlers, and on-disk storage to check
profiles, saves, backups, wiki/map/tutorial links, and dropdown interactions.

On your computer, expand Sastasha and read its tutorial. Open a source link,
choose a city variant for Simply the Hest, and confirm that progress stays
unchanged. Mark one duty, restart the app, and confirm the saved check remains.

v001-v005 remain archived. The private website stays on hold at web v008;
the domain and personal-login setup plan remains paused. GitHub is the planned
distribution service, but no repository upload or public release was made.
The user clarified that Discord did not display an actual warning.

This is an unofficial fan tool. Game references and map artwork belong to
SQUARE ENIX and their respective owners.
