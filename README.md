# foozol - Terminal-First AI Code Assistant Manager

<div align="center">
  <h3><a href="https://github.com/parsakhaz/foozol/releases/latest">**Get the Latest Release Here**</a></h3>
</div>

<div align="center">
  <strong>Terminal-first AI code assistant manager with opinionated UI and full Windows support.</strong>
</div>

<br>

---

## Features

- **Terminal-First Workflow**: Quick access to Terminal (Claude) and Terminal (Codex) for direct CLI interaction
- **Multi-Session Support**: Run multiple Claude Code or Codex instances simultaneously
- **Git Worktree Isolation**: Each session operates in its own isolated git worktree
- **Windows Support**: Full Windows build support with native modules
- **Opinionated UI**: Streamlined interface prioritizing terminal-based workflows

---

## The foozol Workflow

1. Create sessions from prompts, each in an isolated git worktree
2. Iterate with your AI assistant (Claude Code or Codex) inside your sessions
3. Review the diff changes and make manual edits as needed
4. Squash your commits together with a new message and merge to your main branch

---

## Installation

### Download Pre-built Binaries

Download from the [latest release](https://github.com/parsakhaz/foozol/releases/latest):

- **Windows**: `foozol-{version}-Windows-x64.exe` or `foozol-{version}-Windows-arm64.exe`
- **macOS**: `foozol-{version}.dmg`
- **Linux**: `foozol-{version}.AppImage`

### Prerequisites

- **For Claude Code**: Claude Code installed and logged in or API key provided
- **For Codex**: Codex installed (via npm: `@openai/codex`) with ChatGPT account or API key
- Git installed

---

## Building from Source

### Prerequisites

- Node.js 20+
- pnpm
- **Windows**: Visual Studio 2022 Build Tools
- **macOS/Linux**: Xcode Command Line Tools or build-essential

### Build Steps

```bash
# Clone the repository
git clone https://github.com/parsakhaz/foozol.git
cd foozol

# One-time setup
pnpm run setup

# Run in development
pnpm run electron-dev
```

### Building for Production

```bash
# Build for Windows (x64 + arm64)
pnpm build:win

# Build for macOS
pnpm build:mac

# Build for Linux
pnpm build:linux
```

---

## Documentation

For a full project overview, see [CLAUDE.md](CLAUDE.md). Additional documentation can be found in the [docs](./docs) directory.

## License

foozol is open source software licensed under the [MIT License](LICENSE).

## Disclaimer

Claude™ is a trademark of Anthropic, PBC. Codex™ is a trademark of OpenAI, Inc. foozol is not affiliated with, endorsed by, or sponsored by Anthropic or OpenAI.

---

<div align="center">
  By Parsa Khazaeepoul
</div>
