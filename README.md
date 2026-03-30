# LocalSessionManager

[![GitHub Stars](https://img.shields.io/github/stars/Hyggetxc/LocalSessionManager?style=flat-square)](https://github.com/Hyggetxc/LocalSessionManager/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/Hyggetxc/LocalSessionManager?style=flat-square)](https://github.com/Hyggetxc/LocalSessionManager/network/members)
[![GitHub Issues](https://img.shields.io/github/issues/Hyggetxc/LocalSessionManager?style=flat-square)](https://github.com/Hyggetxc/LocalSessionManager/issues)
[![GitHub Pages](https://img.shields.io/badge/demo-online-2f81f7?style=flat-square)](https://hyggetxc.github.io/LocalSessionManager/)

LocalSessionManager is a lightweight local viewer for Codex session files stored in `~/.codex`.

It is especially useful when:

- you use multiple Codex accounts
- some local conversations still exist on disk but do not appear completely in the current Codex sidebar
- you need to inspect the full local conversation history
- you want to generate a handoff package and continue the work in another Codex account without re-explaining everything

## Translations

- [English](./README.md)
- [简体中文](./README.zh-CN.md)

## Demo

- Online: [https://hyggetxc.github.io/LocalSessionManager/](https://hyggetxc.github.io/LocalSessionManager/)
- Repository: [https://github.com/Hyggetxc/LocalSessionManager](https://github.com/Hyggetxc/LocalSessionManager)

## Why This Exists

Codex local session data may still be present in files such as:

- `~/.codex/sessions`
- `~/.codex/archived_sessions`
- `~/.codex/session_index.jsonl`

But the current logged-in account may not fully display those conversations in the desktop sidebar.

This tool is a practical fallback for that situation. It reads the local session files directly in the browser, helps you find the missing conversation, and lets you export a handoff package for a new account or a new thread.

## Features

- Scan local `sessions` and `archived_sessions`
- Search by title, content, session ID, and project directory
- Filter by archive state and project
- Read the full conversation in a cleaner web UI
- Inspect metadata and raw JSONL events
- Browse related sessions in the same project
- Copy or download a handoff package for continuing work in another Codex account
- Light / dark theme and Chinese / English UI

## Usage

1. Open [`index.html`](./index.html) in a Chromium-based browser.
2. Click `Choose .codex`.
3. Select your local `~/.codex` directory.
4. Filter sessions on the left and inspect the full conversation on the right.
5. Use `Copy Handoff` or `Download .txt` when you want to continue in another Codex account.

## Privacy

- All data is processed locally in your browser.
- No session content is uploaded by this tool.
- This tool does not re-import sessions into the current Codex account sidebar.

## Roadmap Ideas

This repository can absolutely grow into a larger project structure, similar to other open-source toolkits.

Possible next additions:

- `docs/` for screenshots, FAQs, and recovery guides
- `examples/` for sample exported handoff packages
- `scripts/` for local utilities or release helpers
- `components/` or `packages/` if the current single-file tool is later split into reusable modules

## Support

If this project helps you recover or continue your Codex conversations, please consider giving it a Star:

- [Star this repository](https://github.com/Hyggetxc/LocalSessionManager)
