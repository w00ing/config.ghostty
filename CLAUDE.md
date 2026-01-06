# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a Ghostty terminal emulator configuration directory. Ghostty is a GPU-accelerated terminal emulator.

## Configuration

The `config` file uses a simple key-value format:
- `key = value` (spacing around `=` is flexible)
- Lines starting with `#` are comments
- Empty values reset options to defaults: `key =`

## Useful Commands

```bash
# View all config options with defaults and documentation
ghostty +show-config --default --docs

# Reload configuration (from within Ghostty)
# Use the keybind or restart the terminal
```

## Documentation

Full configuration reference: https://ghostty.org/docs/config
