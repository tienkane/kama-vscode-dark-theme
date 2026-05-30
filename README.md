# Kama Dark

A warm, low-contrast dark theme for VS Code, based on the brown / cream / gold palette of the **Kama** web app. Designed to be gentle on the eyes with a flat, borderless layout and clear tonal depth between sections.

## Features

- 🤎 Warm brown background with soft cream text — easy on the eyes (editor contrast ~8.5:1, not the harsh 12:1+ of typical dark themes)
- ✨ Muted gold/tan accents instead of bright neon highlights
- 📐 Borderless, flat UI — sections are separated by gentle tonal steps, not hard lines
- 🗂️ Three-tier depth: frame (`#1a1410`) → sidebar/panel (`#211a15`) → editor (`#2a211c`)
- 🎨 Tuned syntax colors, terminal ANSI palette, bracket-pair colors, and git decorations

## Install

### Option A — Clone into the extensions folder (recommended, no build step)

This is the simplest way to use it across machines. VS Code auto-loads any valid extension folder under `~/.vscode/extensions`.

```bash
git clone https://github.com/tienkane/kama-vscode-dark-theme.git ~/.vscode/extensions/kama-dark
```

Then in VS Code:

1. **Reload Window** — `Cmd/Ctrl+Shift+P` → `Developer: Reload Window`
2. **Pick the theme** — `Cmd/Ctrl+K` then `Cmd/Ctrl+T` → select **Kama Dark**

To update later:

```bash
cd ~/.vscode/extensions/kama-dark && git pull
```

### Option B — Build & install a `.vsix`

Requires [`@vscode/vsce`](https://github.com/microsoft/vscode-vsce):

```bash
git clone https://github.com/tienkane/kama-vscode-dark-theme.git
cd kama-vscode-dark-theme
npx @vscode/vsce package
code --install-extension kama-dark-1.0.0.vsix
```

## Palette

| Role | Color |
| --- | --- |
| Frame (activity/title/status/tabs) | `#1a1410` |
| Sidebar / panel | `#211a15` |
| Editor / active tab | `#2a211c` |
| Primary text | `#ccbd9a` |
| Accent (buttons, badges, cursor) | `#b9a482` |
| Keyword | `#c6ac86` |
| String | `#a0a47c` |
| Function | `#cdc0a0` |
| Number / constant | `#c39873` |

## License

[MIT](./LICENSE) © Tien Nguyen
