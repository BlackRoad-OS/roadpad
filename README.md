# RoadPad ✦ BlackRoad OS

[![CI](https://github.com/BlackRoad-OS/roadpad/actions/workflows/ci.yml/badge.svg)](https://github.com/BlackRoad-OS/roadpad/actions/workflows/ci.yml)
[![Python 3.10+](https://img.shields.io/badge/python-3.10%2B-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/github/license/BlackRoad-OS/roadpad)](LICENSE)

> **A clean, distraction-free text editor for BlackRoad OS — powered by Lucidia.**  
> Open it, describe what you want, and start writing. No setup wizards, no config files, no surprises.

---

## ✨ See it in action

```
▗ ▗   ▖ ▖  RoadPad v0.1.0
           Lucidia · BlackRoad OS
  ▘▘ ▝▝

──────────────────────────────────────────────────────────────
>  describe a task to get started
──────────────────────────────────────────────────────────────
  ⏵⏵ accept edits on                              editor mode
```

Type your idea → press **Enter** → your words appear in the editor. That's it.

---

## 🚀 Try it now — one command

```bash
git clone https://github.com/BlackRoad-OS/roadpad.git ~/roadpad
bash ~/roadpad/install-default-surface.sh
source ~/.zshrc
roadpad
```

Open a file directly:

```bash
roadpad notes.road    # open a .road note
roadpad README.md     # open any markdown file
roadpad ideas.txt     # open any text file
```

---

## ⌨️ Controls at a glance

| Key | What it does |
|-----|-------------|
| **Type anything** | Write in the input line |
| **Enter** | Add your text to the document |
| **Shift+Tab** | Switch auto-accept mode (`on` / `review` / `off`) |
| **Ctrl+S** | Save |
| **Ctrl+Q** / **Ctrl+C** | Quit |
| **Arrow keys** | Move around the document |
| **Home** / **End** | Jump to start/end of line |

---

## 📁 Supported file types

| Extension | Description |
|-----------|-------------|
| `.road` | Native BlackRoad notes |
| `.md` | Markdown files |
| `.txt` | Plain text |

---

## 🛠 Default surface setup (optional)

Run this once to make RoadPad your system default editor:

```bash
bash ~/roadpad/install-default-surface.sh
source ~/.zshrc
```

This wires up `EDITOR`, `VISUAL`, and a `blackroad-surface` launcher — so RoadPad opens automatically whenever something asks for a text editor.

---

## 💡 How it works

RoadPad is intentionally simple:

- **You type** in the `>` prompt at the bottom of the screen.
- **Press Enter** — your text lands in the document above.
- **Shift+Tab** lets you control whether edits are applied automatically or need your approval first.
- No AI branding, no popups, no token counters. Just your words.

---

## 📦 What's inside

```
~/roadpad/
├── roadpad.py          ← starts the editor
├── renderer.py         ← draws the screen
├── buffer.py           ← holds your text
├── edit_manager.py     ← manages edit approvals
├── roadpad             ← shell launcher script
└── install-default-surface.sh  ← one-time setup
```

---

## 🔗 BlackRoad OS

RoadPad is part of [BlackRoad OS](https://github.com/BlackRoad-OS) — a minimal, keyboard-first operating environment built around plain text and calm computing.
