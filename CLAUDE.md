# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

**mbot-lektionen** is a set of programming lessons for the **mBot robot** (Makeblock), taught with
the block-based **mBlock 5** IDE at <https://ide.mblock.cc/>. License: Apache 2.0.

The lessons teach block programming from zero. A learner who completes the full course should be able
to program an mBot on their own.

### Audience & pedagogy (hard constraints — do not deviate)

- **Language: German only.** Every lesson, heading, instruction, and code comment is in German. No
  English in lesson bodies. (The `README.md` at repo root and this `CLAUDE.md` stay bilingual/technical.)
- **Readers are self-taught children, ~10+ years old, with zero programming knowledge.** Write for a
  child working alone: warm, encouraging, short sentences, concrete analogies, no jargon without
  explaining it first. Assume no adult is helping.
- **Each lesson is short: 30–60 minutes.**
- **One new programming concept per lesson**, in increasing difficulty. Never introduce two new
  concepts at once. Later lessons build on earlier ones.
- **Every lesson ends with a small, complete program the child runs on the real mBot.** The reward is
  always seeing the robot do something.
- Lessons must be **self-explanatory** — a child reproduces the program by following the steps, without
  external help.

### Concept progression (established; keep consistent when adding lessons)

1. Sequenz + Ereignisse (IDE basics, "wenn mBot startet", LEDs + Ton)
2. Bewegung / Aktion (Motoren: fahren, drehen, anhalten; Parameter Tempo & Zeit)
3. Schleifen (`wiederhole … mal`, `wiederhole fortlaufend`)
4. Sensoren + Bedingung (`Ultraschallsensor`, `falls … dann`)
5. Kombination: `falls … dann … sonst` + Schleife → autonom fahrender Roboter

Beyond 5, continue the ramp: Variablen, Zufall, verschachtelte Schleifen, Linienfolger, Nachrichten/
Broadcasts, eigene Blöcke (Funktionen), Zustände. Full mastery needs more than 5 lessons.

## Repository structure

```
lektionen/
  README.md              Lernpfad / index of all lessons
  00-vorbereitung.md     One-time setup (referenced by every lesson, keeps them short)
  lektion-01-*.md ...     One file per lesson
beispiele/               Optional loadable .mblock example files (see below)
```

## Lesson file conventions

Each lesson file follows the same skeleton (keeps lessons predictable for a child):

- Titel + **Was du lernst** (the one new concept)
- **Was du brauchst** (short; defer full setup to `00-vorbereitung.md`)
- **Das neue Wort / die neue Idee** — the concept explained with an analogy
- **Schritt für Schritt** — numbered build steps naming the exact block *and* its category
- **Dein fertiges Programm** — the whole script shown as an ASCII/indented block listing
- **Probier es aus!** — how to run (Live-Modus vs. Hochladen)
- **Was ist passiert?** — plain explanation of why it works
- **Kleine Herausforderung** — an optional extension
- **Nächste Lektion** — one-line teaser

## mBlock / mBot technical notes

- **IDE:** browser-only at <https://ide.mblock.cc/> (or desktop app). Connect mBot via USB or
  Bluetooth. Set the IDE language to **Deutsch** so block labels match the lessons.
- **Two run modes:** *Live* (blocks run from the computer while tethered — best for testing/learning)
  and *Hochladen/Upload* (firmware flashed so mBot runs untethered). Lessons default to Live and note
  when Upload is nicer.
- **Target hardware:** classic mBot (mCore). Onboard: 2 RGB LEDs, buzzer, button, light sensor, IR.
  Add-ons in the standard kit: ultrasonic sensor (usually port 3) and line follower (usually port 2).
  Lessons 4–5 need the ultrasonic sensor.
- **German block vocabulary used in lessons** (mBlock 5 device = mBot): categories *Ereignisse,
  Aktion, Licht & Ton, Sensoren, Steuerung, Operatoren, Variablen*. Common blocks: `wenn mBot startet`,
  `fahre (vorwärts) mit Tempo ()% für () Sek.`, `anhalten`, `alle eingebauten LEDs leuchten in Farbe ()`,
  `spiele die Note () für () Schläge`, `warte () Sekunden`, `wiederhole () mal`, `wiederhole fortlaufend`,
  `falls < > dann [sonst]`, `Ultraschallsensor Anschluss(3) Entfernung (cm)`.

### `.mblock` example files (`beispiele/`)

- A `.mblock` file is a ZIP archive of a Scratch 3.0 `project.json` (identical structure to `.sb3`)
  plus assets. Import via **Datei → Vom Computer öffnen** in the IDE.
- The mBot hardware blocks are a **device extension**; their exact opcodes (`mbot_...`) are **not
  published anywhere** and only appear inside real exported projects. **Do not hand-author `.mblock`
  files from guessed opcodes** — mBlock will render unknown opcodes as broken/obsolete blocks, which is
  worse for a child than no file.
- To produce reliable loadable examples, first obtain **one real `.mblock` export from the mBlock IDE**
  to use as an opcode/structure template (the user has an ide.mblock.cc account and can export a
  sample). Unzip it, read `project.json`, and mirror its exact opcodes/shadows.
- Until such a template exists, the lessons themselves are the deliverable: a child builds each program
  by hand, which is also the better way to learn block programming.

## MCP / automation

There is **no MCP server for mBlock / Makeblock** (checked Sept 2026). `ide.mblock.cc` has no public
API; it cannot be driven programmatically. Do not attempt to automate the IDE.

## Commit conventions

Follow the repository's git conventions (see the `git-conventions` skill). Commit messages and branch
names per those rules.
