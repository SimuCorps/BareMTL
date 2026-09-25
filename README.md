# BareMTL

BareMTL is a minimal, lightweight desktop code editor. It is a fork of
[Code - OSS](https://github.com/microsoft/vscode) with all AI features and most
extra features removed.

## What is included

- The editor, file explorer, search, and settings
- Integrated terminal
- Git / Source Control
- Debugger (JavaScript debugger built in)
- Tasks
- Language support: TypeScript/JavaScript, JSON, HTML, CSS, Markdown (with preview), Emmet
- Themes, grammars, and snippets
- Welcome page and walkthroughs

## What is removed

- All AI features: chat, inline chat, agents, MCP, Copilot, speech and voice, AI search
- Telemetry and experiments
- Settings Sync, edit sessions, and the profiles UI
- Notebooks / Jupyter
- Testing and Timeline views
- Web, server, remote, and tunnel targets (BareMTL is Electron desktop only)
- The extension marketplace and the Extensions view. The extension host still runs
  the bundled built-in extensions only.

## Building

Requires the Node.js version in [`.nvmrc`](.nvmrc).

```sh
npm ci
npm run compile
./scripts/code.sh
```

Package a build for the current platform, for example Linux x64:

```sh
npm run gulp vscode-linux-x64-min
```

## License

BareMTL is Copyright (c) 2026 - present [SimuCorps](https://simucorps.org).

BareMTL is built from Code - OSS, Copyright (c) 2015 - present Microsoft Corporation.
Licensed under the [MIT](LICENSE.txt) license. Third-party notices are in [ThirdPartyNotices.txt](ThirdPartyNotices.txt).
