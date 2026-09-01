# Changelog

What changed in Inkgrove, written for the person writing in it.

Installers live on the
[releases page](https://github.com/capactiyvirus/inkgrove/releases). A version
marked **coming** is finished and being tested, and is not yet a build you can
download.

---

## 0.9.0 — coming

The version that can update itself. From here on a new build arrives inside the
app, so 0.9.0 is the last one you have to come and fetch by hand.

### New

- **Updates install themselves, when you say so.** Inkgrove notices a new
  version, you press Download, and then Install and restart. It never installs
  on its own and it never restarts without being asked. Before it swaps
  anything, your work is saved and your library is backed up, and if that backup
  cannot be taken the update is refused rather than going ahead without one. It
  is off by default, and Settings → About is where you turn it on.

- **Duplicate characters and places can be folded back into one.** An import
  makes one sheet per file, so the same person can arrive three times, as a
  first name, a full name and a nickname. Press **Select** at the top of the
  Characters or World list to bring out the tick boxes, tick the duplicates
  (Shift-click takes a whole run), press Merge, and choose which one keeps its
  name. Everything you typed on the others moves across: their text is added to
  the matching box under a line saying which sheet it came from, their pictures
  follow, your `[[links]]` are re-pointed, and the survivor answers to all of
  the old names, so prose that used them still lights up. You read exactly what
  is about to happen before it happens, and the sheets you folded in wait in the
  Trash in case you change your mind.

- **A book you delete can come back.** Deleting a book or a notebook used to be
  permanent. It now goes to the library's Trash with everything inside it
  intact, and restoring puts it back on its shelves. Emptying the trash is the
  only step that removes anything, and it says so before it does.

- **A portrait can be changed.** Once a character or place had a picture there
  was no way to swap it, since clicking only opened the viewer. There is now a
  **Change picture** button under the portrait. It is a reorder rather than a
  delete, so the picture it replaces keeps its place in Images.

- **Word lookup answers again.** The dictionary Inkgrove asked first stopped
  responding in late August, and because it was first in line every lookup sat
  waiting on it before trying anywhere else. Wiktionary has been added as a
  third source and now goes first, so a definition arrives in well under a
  second, with senses grouped by part of speech and examples where the entry
  has them.

### Fixed

- **Names in the Characters and World lists were being cut short**, because
  buttons that only appear on hover were taking up room even while hidden.
- **The sheet you had open looked the same as whatever you were hovering.** It
  now carries a gold bar down its left edge, which stays put when the pointer
  moves away.
- **On a touchscreen the list header sat at three different heights**, and two
  of its controls were too small to tap reliably.
- **Research notes sometimes opened blank**, and clicking away and back was the
  only way to see the text.
- **Keyboard hints showed Mac shortcuts on Windows.** Tooltips, the menu bar and
  the shortcuts sheet now say Ctrl where Ctrl is what you press.
- **Emptying the library trash left tabs open on scenes that no longer existed.**
  Purging a book now closes everything that belonged to it.
- On macOS the update notice overlapped the window buttons.

---

## 0.8.260 — released 2026-08-29

Inkgrove is **beta** now. Same promise underneath: your writing stays on your
machine, in files you own, with no account and no server holding any of it.

### New

- **News in your library.** A quiet section below your books where you hear what
  changed and what is coming. Fold it away by clicking the heading and it stays
  folded. It can be switched off entirely, and when it is off nothing is fetched
  at all.
- **A newsletter, if you want one.** Settings → About → Newsletter opens a
  Substack page in your own browser. There is no signup form in the app and the
  app itself never contacts Substack, so if you do subscribe, your email address
  never reaches Inkgrove.
- **Edit and reset your writing history.** Click any square in the library
  heatmap to correct a day, or reset the whole record. Hand-adjusted days are
  marked as such.
- **Pick your dictionary.** Settings → Editor → Word lookup. A source that stops
  answering is greyed out, and lookups fall through to one that works instead of
  hanging.
- **Settings headings collapse**, so a long panel is an index instead of a wall.

### Fixed

- **The writing tracker was losing your time.** Minutes were counted as spent
  before the write meant to store them, and a write that failed was swallowed in
  silence, so "Time today" and the heatmap could sit empty while you were
  visibly working. On the desktop app closing the window fired neither of the
  hooks the tracker relied on, so the tail of every session went in the bin.
- **Your best days were invisible** in the Goals chart. Days that hit your daily
  target were painted in a colour that does not exist, so they drew as nothing
  at all.
- **Help tooltips were sliced off** by the edge of whatever panel they opened
  in, so you got half a sentence.
- **The light candle and aurora backgrounds looked like a stain**, and text over
  the sepia light background was below the contrast standard the rest of the app
  is held to.
- **Loading a sample no longer invents a fortnight of writing history.** The
  heatmap and your streaks are a record of showing up, not a screenshot prop.

---

Older history is in the
[release notes](https://github.com/capactiyvirus/inkgrove/releases) for each
build.
