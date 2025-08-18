# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a VS Code theme extension called "Eidolon Root" - a dark theme designed for clarity and comfort with bold contrast and vibrant accents.

## Key Files and Structure

- `themes/Eidolon Root-color-theme.json` - Main theme definition file containing all color settings for the editor UI and syntax highlighting
- `package.json` - Extension manifest defining the theme contribution and VS Code version requirements
- `src-theme/root.txt` - Source color palette in a simplified format (appears to be from a terminal color scheme)

## Development Commands

### Testing the Theme
- Press `F5` in VS Code to launch an Extension Development Host window with the theme loaded
- Use `Preferences: Color Theme` command (`Ctrl+K Ctrl+T` or `Cmd+K Cmd+T` on Mac) to select the theme
- Use `Developer: Inspect Editor Tokens and Scopes` to examine token scopes when editing the theme

### Installation
- Copy the extension folder to `<user home>/.vscode/extensions` for local installation
- Changes to the theme JSON file are automatically applied to the Extension Development Host window

## Theme Architecture

The theme follows VS Code's standard theming architecture:
- **UI Colors**: Defined in the `colors` object (editor background, sidebar, activity bar, tabs)
- **Syntax Highlighting**: Defined in the `tokenColors` array using TextMate scopes
- **Color Palette**: Based on a 16-color terminal palette (0-15) defined in `src-theme/root.txt`

Key color values from the palette:
- Background: `#151719`
- Foreground: `#e4e5df`
- Primary accent: `#f6b34c` (yellow/orange)
- Secondary accents: `#83e96c` (green), `#c89ef0` (purple), `#3ad4b7` (cyan)

## Publishing

To publish updates to the VS Code marketplace, refer to: https://code.visualstudio.com/api/working-with-extensions/publishing-extension