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
| **Windows 10/11 (x64)** | ✅ Available | `Inkgrove_<version>_x64-setup.exe` (recommended) or `Inkgrove_<version>_x64_en-US.msi` |
| **macOS (Intel & Apple silicon)** | ✅ Available | `Inkgrove_<version>_universal.dmg` |
| **iOS / Android** | 🔜 Planned | — |

Not every release carries every asset — check the release you're downloading. No installer
for your OS? Use the free **browser demo** — no install, runs entirely in your browser:
**https://inkgrove.app**

### Your OS will warn on first run
Inkgrove is in **alpha** and not yet code-signed, so your OS can't verify who made the
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

- **📝 Distraction-free editor** — a clean, paginated writing surface with focus mode.
- **📑 Chapter binder** — organize your manuscript into chapters and scenes, drag to reorder.
- **🗂️ Corkboard** — see your scenes as index cards; rearrange the structure visually.
- **🧭 Outline** — a bird's-eye view of the whole book, with per-scene synopses.
- **📖 Story Bible** — track **characters**, **world** details, and **research** in one place,
  linked to where they appear.
- **🧩 Plot grid** — map plot threads across chapters so nothing gets dropped.
- **🔍 Project-wide search** — find any line across the entire manuscript instantly.
- **🕘 Scene snapshots** — automatic versions of your scenes, so an edit is never final.
- **🎯 Writing goals** — set a manuscript word target and a daily goal; a streak keeps
  you honest.
- **📅 Writing history** — a grid of the last 16 weeks in the library. Any day you showed
  up gets a shade, not just days you added words, so a hard revision day isn't blank.
- **🗄️ A library, not a list** — group books onto shelves, and browse a shelf's whole
  cast, world, or notes in one place.
- **🗑️ Trash & restore** — deleting a chapter, scene, character, or note puts it in that
  book's trash, where you can put it back.
- **📥 Import your work** — drop in a folder of `.docx` / `.md` / `.txt`, or a Scrivener
  project, and Inkgrove sorts it into chapters (and can extract characters, world, and
  plot for you).

---

## Local-first & private

Your writing **never leaves your machine** unless you choose to move it.

- **On disk, in your control** — the desktop app stores your work as a real database
  file on your computer (`inkgrove.db`), not in a cloud you don't own.
- **No account, no sign-up, no telemetry of your text.** There is no server to send it to.
- **Fully offline.** Write on a plane; nothing depends on a connection.
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
These survive app updates. To move Inkgrove to a new machine, copy `inkgrove.db`.

---

## Cross-device, your way

No proprietary sync, and none planned. To get your manuscript onto a second machine today:
**export** it (an `.inkgrove` bundle, or Markdown), or **copy `inkgrove.db`** into a folder
inside **your own Dropbox / iCloud / Google Drive** and pull it down on the other side. Your
data, your account, no middleman.

Inkgrove can't yet be pointed at a folder of your choosing, and it won't keep two machines
in step for you. A **vault** — your writing mirrored as real `.md` files in a folder you
keep — is on the roadmap and is how this is meant to work.

---

## Status

**Alpha.** Inkgrove is under active development and improving fast.

- Back up your work (the app's Export, plus your own cloud folder) so a cleared install or
  disk failure can't cost you the novel.
- Expect rough edges; please [report issues](https://github.com/capactiyvirus/inkgrove/issues).

---

## On the roadmap

- Native mobile apps
- **Story Map** — see your whole book at a glance
- Higher-fidelity import from more formats and sources
- Code-signed installers

---

<div align="center">

**[Download](https://github.com/capactiyvirus/inkgrove/releases/latest)** ·
**[Browser demo](https://inkgrove.app)** ·
**[Report an issue](https://github.com/capactiyvirus/inkgrove/issues)**

*Inkgrove — your novel, on your machine, in a file you own.*

</div>
