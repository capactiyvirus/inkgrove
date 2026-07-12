<div align="center">

<img src="assets/banner.png" alt="Inkgrove" width="620" />

### Write your novel. It stays yours.

A complete, **local-first** writing studio for long-form fiction — as a free desktop app.
No account. No upload. No server. Your words live on your machine.

[**⬇ Download the latest release**](https://github.com/capactiyvirus/inkgrove/releases/latest) &nbsp;·&nbsp; [Try the browser demo](https://lit-haven.pages.dev)

</div>

> **This repository hosts the public releases of Inkgrove.** The application source is
> maintained privately; grab the installer from [Releases](https://github.com/capactiyvirus/inkgrove/releases/latest).

---

## Why Inkgrove

Inkgrove sits between the heavyweight desktop organizers and the build-it-yourself
note vaults: **novel-shaped structure, files you own, zero setup, free to start.**
Chapters, scenes, a Story Bible, and plot tools are built in from the first minute —
and everything exports to open formats, so leaving is always one click away.
That's the deal: we earn your stay, we never lock the door.

---

## Download & install

| Platform | Status | Asset |
|---|---|---|
| **Windows 10/11 (x64)** | ✅ Available | `Inkgrove_<version>_x64-setup.exe` (recommended) or `Inkgrove_<version>_x64_en-US.msi` |
| **macOS** | 🟡 Older build available | `Inkgrove_0.8.77_universal.dmg` (see [releases](https://github.com/capactiyvirus/inkgrove/releases)) — a current-version build ships with the next release (both platforms now build in CI) |
| **Linux** | 🔜 Coming soon | — |
| **iOS / Android** | 🔜 Planned | the **browser demo** already works on phones today |

No installer for your OS yet? Use the free **browser demo** — no install, runs entirely
in your browser: **https://lit-haven.pages.dev**

### Windows: "Windows protected your PC"
Inkgrove is in **alpha** and not yet code-signed, so Windows SmartScreen may flag it as
from an *unrecognized publisher*. This is expected for a new app, not a virus warning —
click **More info → Run anyway**. Code signing is on the roadmap.

### macOS: "app can't be opened"
Same story on the Mac: an unsigned app needs one manual allow — right-click the app →
**Open** → **Open** (or System Settings → Privacy & Security → **Open Anyway**).

After installing, launch **Inkgrove** from the Start menu / Applications. On first run it
shows a short welcome, then drops you into your projects.

---

## What it is

Inkgrove is a full novel-writing environment — not a note-taking app with a word count.
Everything a long manuscript needs, in one place:

- **📝 A real writing editor** — clean prose surface with **focus**, **typewriter**, and
  **distraction-free** modes, manuscript-standard fonts and sizes.
- **📑 Chapter binder** — nested chapters and scenes, drag to reorder or restructure.
- **🗂️ Corkboard** — your scenes as index cards on a freeform board; pan, zoom, star,
  and comment your way to a structure.
- **🧭 Outline** — a bird's-eye table of the whole book, with per-scene status, POV,
  and synopses.
- **🗺️ Story Map** — the whole narrative on one timeline-style map.
- **📖 Story Bible** — track **characters**, **world** details, and **research** alongside
  the manuscript. Character sheets with portraits, goals, conflicts, and voice notes.
- **✨ Names light up in your prose** — mention a character or place you've recorded and
  it gets a subtle underline; hover it for their reference card (portrait + who they are),
  or `[[wiki-link]]` anything and follow backlinks both ways.
- **🧩 Plot grid** — map plot threads across chapters so nothing gets dropped.
- **🔍 Project-wide search** — find any line across the entire manuscript instantly.
- **🕘 Scene snapshots** — automatic versions with readable diffs, so an edit is never
  final and a bad rewrite is one restore away.
- **🎯 Writing goals** — a manuscript target and a daily goal, with streaks (and a
  little fire) to keep you honest.
- **✔️ Spell check & word lookup** — in-app spelling with a personal dictionary, plus
  Alt+click any word for definitions and synonyms. Fully offline.
- **📥 Import your work** — drop in `.docx` / `.md` / `.txt` / a whole folder or ZIP,
  a **Scrivener project** (`.scriv`), or one big Google-Docs export — Inkgrove splits it
  into chapters and scenes for review before anything is created (and can propose
  characters, world entries, and plot threads from the draft).
- **🌗 Dark mode & themes** — including guided tours to find your way around.

## No lock-in — the exit door is built in

Your manuscript exports to **open formats**, whole-book or per-project, no strings:

- **DOCX** (Word), **EPUB**, **PDF**, and **plain text**
- **Markdown vault** — an Obsidian-style folder of `.md` files (chapters → folders,
  scenes → files with front-matter), zipped
- **`.inkgrove` bundle** — the complete project (manuscript + Story Bible + images) in
  one portable file; re-import it anywhere, including the browser demo

If Inkgrove disappeared tomorrow, your book walks out in formats everything else reads.

---

## Local-first & private

Your writing **never leaves your machine** unless you choose to move it.

- **On disk, in your control** — the desktop app stores your work as a real database
  file on your computer (`inkgrove.db`), not in a cloud you don't own.
- **No account, no sign-up, no telemetry of your text.** There is no server to send it to.
  (Optional, opt-in crash reports exist — they never contain your writing.)
- **Fully offline.** Write on a plane; nothing depends on a connection.
- **Automatic backups** — the app keeps rolling local backups so a bad edit, crash, or
  corruption is recoverable.

### Where your data lives (Windows)
```
Your library:   %LOCALAPPDATA%\app.inkgrove.desktop\inkgrove.db
Backups:        %LOCALAPPDATA%\app.inkgrove.desktop\backups\
Settings:       %APPDATA%\app.inkgrove.desktop\config.json
```
These survive app updates. To move Inkgrove to a new machine, copy `inkgrove.db`.

---

## Your own AI (bring your own key)

Inkgrove has a **manuscript-aware AI** that you power with **your own Anthropic API key** —
so you pay the AI provider directly and **we never see your key or your writing**.

- Paste your key in **⚙ Settings** (session-only by default) and pick a model
  (Claude Haiku / Sonnet / Opus).
- **Scene & book synopsis** — summarize what you've written.
- **Build from manuscript** — the AI reads your draft and *proposes* characters, world
  entries, and plot threads for you to review and apply.
- An **AI history** log shows what ran and the token spend.
- No key? Everything else works exactly the same — the AI is optional, not the product.

**The principle:** AI **assists** — it reads, summarizes, and organizes. It **never writes
your prose for you**. The book stays yours.

---

## Cross-device, your way

No proprietary sync. If you want your manuscript on more than one machine, point Inkgrove's
files at a folder inside **your own Dropbox / iCloud / Google Drive** — your cloud carries
it across devices. Your data, your account, no middleman.

---

## Status

**Alpha.** Inkgrove is under active development and improving fast.

- Back up your work (the app's Export, plus your own cloud folder) so a cleared install or
  disk failure can't cost you the novel.
- Expect rough edges; please [report issues](https://github.com/capactiyvirus/inkgrove/issues).

---

## On the roadmap

- One consolidated release for **Windows + macOS**, then **Linux**
- **Vault folder** — live-mirror your manuscript into a folder of real Markdown files you
  own (works beautifully next to an Obsidian vault), with reviewed pull-back of outside edits
- Native mobile apps
- Deeper import fidelity (Scrivener metadata, more formats)
- Code-signed installers

---

<div align="center">

**[Download](https://github.com/capactiyvirus/inkgrove/releases/latest)** ·
**[Browser demo](https://lit-haven.pages.dev)** ·
**[Report an issue](https://github.com/capactiyvirus/inkgrove/issues)**

*Inkgrove — a writing tool that assists, and never writes your prose for you.*

</div>
