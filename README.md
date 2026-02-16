# Haptix

The Haptix macOS companion app enables AI agents to interact with iOS devices and simulators through the Model Context Protocol (MCP).

## Installation

1. Download the latest `Haptix.dmg` from [Releases](https://github.com/haptix-dev/app/releases)
2. Open the DMG and drag **Haptix** to your Applications folder
3. Launch Haptix from your Applications folder

## Getting Started

Haptix runs as a menu bar app. After launching:

1. **Enter your license key** in Settings > License
2. **Add your MCP configuration** to your AI agent (Claude, Codex, Cursor, etc.)
3. **Connect a device** — Haptix discovers iOS devices running the HaptixKit SDK via Bonjour

### MCP Configuration

Add the following to your agent's MCP settings:

```json
{
  "mcpServers": {
    "haptix": {
      "url": "http://localhost:4278/mcp"
    }
  }
}
```

The default port is `4278` and can be changed in Settings > General.

## Requirements

- macOS 26.0 or later
- A valid Haptix license key
- iOS app(s) integrating the [HaptixKit SDK](https://github.com/haptix-dev/sdk)

## Features

- **Menu bar app** with a dockable main window
- **Multi-device support** — connect and manage multiple iOS devices simultaneously
- **Per-device logging** — filter logs by device or view all at once
- **MCP server** — exposes device interaction tools to AI agents
- **Bonjour discovery** — automatically finds devices on the local network
- **License management** — per-seat licensing with activation/deactivation
- **Pairing security** — optional pairing code verification between app and device

## Support

For questions and support, visit [haptix.dev](https://haptix.dev).
