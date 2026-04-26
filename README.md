# 🧠 AI Personal Assistant

> A 360° autonomous personal assistant built on Obsidian, Claude, and Google Workspace — capturing everything, forgetting nothing, running round the clock.

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://python.org)
[![Claude API](https://img.shields.io/badge/Claude_API-D97757?style=flat&logo=anthropic&logoColor=white)](https://anthropic.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Status: Active](https://img.shields.io/badge/Status-Active-brightgreen)](.) 

---

## What this is

A personal knowledge management system that acts as an always-on assistant. It connects Gmail, Google Calendar, and Google Drive to a structured Obsidian vault — automatically briefing you every morning, capturing action items, and keeping your second brain up to date without manual effort.

**Core idea:** Your assistant should work even when you're asleep.

---

## Features

- **Daily morning briefing** — auto-generated note with today's calendar + priority inbox every day at 7 AM
- **PARA vault structure** — Inbox, Projects, Areas, Resources, Archive with consistent templates
- **Gmail integration** — surface action items and priority threads directly into notes
- **Calendar sync** — pull meetings into daily notes and generate meeting note stubs
- **Drive integration** — read and write documents from within the knowledge system
- **5 note templates** — Daily, Meeting, Capture, Project, Weekly Review

---

## Architecture

```
Gmail + Calendar + Drive
         │
    Claude (AI layer)
         │
    Obsidian Vault (local markdown)
    ├── 00 - Inbox
    ├── 01 - Projects
    ├── 02 - Areas
    ├── 03 - Resources
    ├── 04 - Archive
    ├── 05 - Daily Notes   ← auto-generated daily
    └── 06 - Templates
```

---

## Getting started

```bash
# Clone this repo
git clone https://github.com/saugangu11/ai-personal-assistant.git

# Open the vault in Obsidian
# File → Open Folder as Vault → select this directory
```

**Requirements:**
- [Obsidian](https://obsidian.md) (free)
- Claude Cowork or Claude API access
- Google Workspace account (Gmail, Calendar, Drive)

---

## Roadmap

- [ ] Obsidian Local REST API integration for direct vault writes
- [ ] Weekly review automation (Sunday 6 PM)
- [ ] Slack / Teams integration for message capture
- [ ] Smart tagging and auto-linking of notes
- [ ] Mobile quick-capture shortcut

---

## License

MIT — use it, fork it, build on it.
