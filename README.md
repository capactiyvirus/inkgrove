<div align="center">

<img src="assets/banner.png" alt="Inkgrove" width="620" />

### Write your novel. It stays yours.

A complete, **local-first** writing studio for long-form fiction — as a free desktop app.
No account. No upload. No server. Your words live on your machine.

[**⬇ Download the latest release**](https://github.com/capactiyvirus/inkgrove/releases/latest) &nbsp;·&nbsp; [Try the browser demo](https://inkgrove.app)

</div>

> **This repository hosts the public releases of Inkgrove.** The application source is
> maintained privately; grab the installer from [Releases](https://github.com/capactiyvirus/inkgrove/releases/latest).

---

## Download & install

| Platform | Status | Asset |
|---|---|---|
| **Windows 10/11 (x64)** | ✅ Available | `Inkgrove_<version>_x64-setup.exe` |
| **macOS (Intel & Apple silicon)** | ✅ Available | `Inkgrove_<version>_universal.dmg` |
| **iOS / Android** | 🔜 Planned | — |

### There is a beta ahead of the stable release

The download button above gives you the current stable build. **0.9.0 is out as a
beta** if you would like the newest work early, and it is where the features marked
*0.9.0* below live: updates that install themselves, merging duplicate characters and
places, a trash for whole books, and replacing a portrait. It is a beta because an
update mechanism is the one feature that cannot really be tested alone, and it leaves
your existing library exactly as it is.

**[Get the 0.9.0 beta](https://github.com/capactiyvirus/inkgrove/releases/tag/v0.9.0)**

Not every release carries every asset, so check the release you're downloading. No installer
for your OS? The free **browser demo** runs entirely in your browser with nothing to install,
though it's a test drive rather than somewhere to keep a novel: it holds one project of up to
5,000 words, and it keeps your writing in memory only, so closing or reloading the tab clears
it. **https://inkgrove.app**

### Your OS will warn on first run
Inkgrove is in **beta** and not yet code-signed, so your OS can't verify who made the
app. The warning is about identity, not a virus alert — it's expected for a new unsigned
app. Code signing is on the roadmap.

- **Windows** — SmartScreen says "Windows protected your PC": click
  **More info → Run anyway**.
- **macOS** — Gatekeeper says Inkgrove can't be opened because Apple can't verify it.
  Double-click the app, click **Done** on the warning, then open
  **System Settings → Privacy & Security**, scroll to **Security**, and next to the
  *"Inkgrove" was blocked* message click **Open Anyway** — confirm with your password or
  Touch ID. macOS 15 (Sequoia) removed the old Control-click → Open shortcut, so this is
  the way through.

After installing, launch **Inkgrove**. On first run it shows a short welcome, then drops
you into your projects.

---

## What it is

Inkgrove is a full novel-writing environment — not a note-taking app with a word count.
Everything a long manuscript needs, in one place:

- **📝 Distraction-free editor** — a clean writing surface shaped like a manuscript page,
  with focus mode.
- **📑 Chapter binder** — organize your manuscript into chapters and scenes, drag to reorder.
- **🗂️ Corkboard** — see your scenes as index cards; rearrange the structure visually.
- **🧭 Outline** — a bird's-eye view of the whole book, with per-scene synopses.
- **📖 Story Bible** — track **characters**, **world** details, and **research** in one place,
  linked to where they appear. A sheet's portrait can be swapped from the sheet itself *(0.9.0)*, and
  the picture it replaces keeps its place in that sheet's images.
- **🔀 Merge duplicates** *(0.9.0)* — an import can leave the same person on three sheets, as a first
  name, a full name and a nickname. Tick them in the Characters or World list, press Merge,
  and choose which one keeps its name: everything you typed on the others moves across, the
  survivor answers to all of the old names, your `[[links]]` are re-pointed, and the sheets
  you folded in wait in the trash in case you change your mind.
- **🔍 Project-wide search** — find any line across the entire manuscript instantly.
- **🕘 Scene snapshots** — automatic versions of your scenes, so an edit is never final.
- **🎯 Writing goals** — set a manuscript word target and a daily goal; a streak keeps
  you honest.
- **📅 Writing history** — a grid of the last 16 weeks in the library. Any day you showed
  up gets a shade, not just days you added words, so a hard revision day isn't blank.
- **🗄️ A library, not a list** — group books onto shelves, and browse a shelf's whole
  cast, world, or notes in one place.
- **🗑️ Trash & restore** — deleting a chapter, scene, character, or note puts it in that
  book's trash, and *(0.9.0)* deleting a whole book or notebook puts it in the library's trash with
  everything inside it untouched, so restoring gives you the book back on its shelves with
  the same chapters in the same order. Emptying the trash is the only step that removes
  anything, and it says so first.
- **📥 Import your work** — drop in `.docx` / `.md` / `.txt` / `.rtf` files, a whole folder
  of them, a `.zip`, or a Scrivener project, and Inkgrove sorts it into chapters and scenes
  by your folder structure, or by the headings inside one long file, with a review step where
  you rename and re-target everything before a single record is created. Files you put in a
  `characters`, `world` or `research` folder become Story Bible sheets. Afterwards **Scan for
  names** reads the manuscript on your own machine for likely character and place names and
  offers them as a checklist, so nothing joins your Story Bible that you didn't tick.
- **🔤 Word lookup** — Alt-click any word in your prose for definitions and synonyms without
  leaving the page.
- **🔄 Updates that install themselves** *(0.9.0)* — Inkgrove notices a new version, you press Download,
  then Install and restart. It never installs on its own and it never restarts without being
  asked, and before it swaps anything it saves your work and backs up your library, refusing
  the update rather than going ahead if that backup can't be taken.

---

## Local-first & private

Your writing **never leaves your machine** unless you choose to move it.

- **On disk, in your control** — the desktop app stores your work as a real database
  file on your computer (`inkgrove.db`), not in a cloud you don't own.
- **No account, no sign-up, and no telemetry of your text.** There is no server to send it to.
- **Crash reports and usage counters exist, and each is opt-in and off by default.** Neither
  can carry your writing: a crash report is the error and a stack trace with your username
  scrubbed out of the paths, and a usage counter is a named event with a bucketed number, so
  prose, titles, character names and search queries never leave your device. Both switches
  live in **Settings → About → Privacy**, alongside the news panel, which is the one network
  feature that's on by default and only ever reads one small public file.
- **Writing works offline.** Nothing you do to a manuscript needs a connection. The parts
  that reach the network are word lookup, which sends the single word you asked about and
  nothing else, the update check, and that news panel.
- **Automatic backups** (desktop) — the app copies your library on launch and keeps a
  rolling set, so a bad edit, crash, or corruption is recoverable. **Settings → Storage**
  controls it: how many to keep, how often, an optional size limit, and an off switch.
  One verified-good copy is pinned outside the rotation and never rotated away.

### Where your data lives (Windows)
```
Your library:   %LOCALAPPDATA%\app.inkgrove.desktop\inkgrove.db
Backups:        %LOCALAPPDATA%\app.inkgrove.desktop\backups\
Settings:       %APPDATA%\app.inkgrove.desktop\config.json
```
These survive app updates. To move Inkgrove to a new machine, close the app first so the
last of your writing is folded back into that one file, then copy `inkgrove.db`.

---

## Cross-device, your way

No proprietary sync, and none planned. To get your manuscript onto a second machine today:
**export** it (an `.inkgrove` bundle, or Markdown), or **close Inkgrove and copy
`inkgrove.db`** into a folder inside **your own Dropbox / iCloud / Google Drive**, then pull
it down on the other side. Your data, your account, no middleman.

Inkgrove can't yet be pointed at a folder of your choosing, and it won't keep two machines
in step for you. A **vault** — your writing mirrored as real `.md` files in a folder you
keep — is on the roadmap and is how this is meant to work.

---

## Status

**Beta.** Inkgrove is under active development and improving fast.

- Back up your work (the app's Export, plus your own cloud folder) so a cleared install or
  disk failure can't cost you the novel.
- Expect rough edges; please [report issues](https://github.com/capactiyvirus/inkgrove/issues).

---

## On the roadmap

- Native mobile apps
- **Story Map** — see your whole book at a glance, with the **plot grid** that maps threads
  across chapters as its table view
- A **vault** — your writing mirrored as real files in a folder you keep
- Higher-fidelity import from more formats and sources, including character sheets whose
  fields land in the matching fields
- Code-signed installers

---

<div align="center">

**[Download](https://github.com/capactiyvirus/inkgrove/releases/latest)** ·
**[Browser demo](https://inkgrove.app)** ·
**[Report an issue](https://github.com/capactiyvirus/inkgrove/issues)**

*Inkgrove — your novel, on your machine, in a file you own.*

</div>
