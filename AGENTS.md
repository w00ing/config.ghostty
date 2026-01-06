# Repository Guidelines

## Project Overview
This repository contains a single Ghostty terminal configuration. The primary artifact is the `config` file, which sets UI, keybindings, and typography options.

## Project Structure & Module Organization
- `config`: Main Ghostty configuration (key-value pairs). Group related settings with comment headers.
- `CLAUDE.md`: Agent-specific instructions for working in this repo.

## Build, Test, and Development Commands
- `ghostty +show-config --default --docs`: Print all available settings with defaults and documentation.
- Reload config: restart Ghostty or use your configured reload keybinding (if present).

## Coding Style & Naming Conventions
- Use one setting per line: `key = value` (spacing around `=` is flexible, prefer `key = value`).
- Comments start with `#` on their own line; inline comments are not supported after a setting.
- Quote strings that contain spaces: `font-family = "JetBrains Mono"`.
- Keep sections ordered by intent (e.g., cursor, keybinds, aesthetics, typography) and separate with blank lines.

## Testing Guidelines
- No automated tests in this repository.
- Manual verification: open Ghostty and confirm behavior (cursor style, keybinds, opacity). Use `ghostty +show-config --default --docs` to check defaults when comparing changes.

## Commit & Pull Request Guidelines
- No commit history exists yet, so no established convention. Use concise, imperative subjects (e.g., `config: adjust font size`).
- PRs should explain the user-facing effect, list changed settings, and include screenshots if visuals change (opacity, blur, fonts).

## Security & Configuration Tips
- Avoid storing secrets or tokens in the config file.
- Be careful with keybindings that send control sequences (tmux/ssh) and document their intent in nearby comments.

## Agent-Specific Instructions
- Read `CLAUDE.md` before making changes; it describes repo-specific conventions and Ghostty references.
