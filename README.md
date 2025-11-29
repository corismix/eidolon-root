# Eidolon Root

A high-contrast dark theme featuring a deep matte background, vibrant pastel syntax highlighting, and a distraction-free UI designed for long coding sessions.

## Build & Publish

### Prerequisites
Ensure you have [Node.js](https://nodejs.org/) installed.

### Build (`.vsix`)
To create a package file (`.vsix`) for manual installation:

```bash
npx vsce package
```

## Installation

### Local `.vsix` Installation
1.  Download the `.vsix` file from the [releases page](https://github.com/corismix/eidolon-root/releases) or build it yourself using the instructions above.
2.  Open VS Code.
3.  Go to the Extensions view (`Ctrl+Shift+X` / `Cmd+Shift+X`).
4.  Click on the `...` (More Actions) menu at the top right of the Extensions sidebar.
5.  Select `Install from VSIX...`
6.  Navigate to and select the downloaded `.vsix` file.

## Publish

#### VS Code Marketplace
1. Create a [Personal Access Token](https://code.visualstudio.com/api/working-with-extensions/publishing-extension#get-a-personal-access-token) (PAT).
2. Create a publisher: https://marketplace.visualstudio.com/manage
3. Log in and publish:

```bash
npx vsce login <publisher id>
npx vsce publish
```

#### OpenVSX Registry
1. Create a token at [open-vsx.org](https://open-vsx.org/user-settings/tokens).
2. Create a namespace: https://open-vsx.org/user-settings/namespaces
3. Publish:

```bash
npx ovsx publish -p <token>
```
