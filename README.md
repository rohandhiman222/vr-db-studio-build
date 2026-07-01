<div align="center">
  <h1>VR DB Studio</h1>
  <p>Desktop database client for PostgreSQL, MySQL, SQLite, SQL Server, Oracle, MongoDB &amp; Redis<br/>with built-in <strong>Claude AI MCP server</strong></p>
  <img src="https://img.shields.io/github/v/release/rohandhiman222/vr-db-studio-build?label=latest&color=0ea5e9" alt="Latest Release"/>
  &nbsp;
  <img src="https://img.shields.io/badge/platforms-Linux%20%7C%20Windows%20%7C%20macOS-6366f1" alt="Platforms"/>
</div>

---

## Download

| Platform | Download | Description |
|----------|----------|-------------|
| **Linux** (Ubuntu/Debian) | [vr-db-studio-linux-amd64.deb](https://github.com/rohandhiman222/vr-db-studio-build/releases/latest/download/vr-db-studio-linux-amd64.deb) | App + MCP server |
| **Windows** | [vr-db-studio-windows-amd64-installer.exe](https://github.com/rohandhiman222/vr-db-studio-build/releases/latest/download/vr-db-studio-windows-amd64-installer.exe) | Desktop app installer |
| **Windows MCP only** | [vr-db-mcp-server-windows-amd64.exe](https://github.com/rohandhiman222/vr-db-studio-build/releases/latest/download/vr-db-mcp-server-windows-amd64.exe) | MCP server binary |
| **macOS** (Universal) | [vr-db-studio-macos.zip](https://github.com/rohandhiman222/vr-db-studio-build/releases/latest/download/vr-db-studio-macos.zip) | Intel + M1/M2/M3 |
| **macOS MCP (M1/M2/M3)** | [vr-db-mcp-server-darwin-arm64](https://github.com/rohandhiman222/vr-db-studio-build/releases/latest/download/vr-db-mcp-server-darwin-arm64) | MCP server binary |
| **macOS MCP (Intel)** | [vr-db-mcp-server-darwin-amd64](https://github.com/rohandhiman222/vr-db-studio-build/releases/latest/download/vr-db-mcp-server-darwin-amd64) | MCP server binary |

> All releases: [github.com/rohandhiman222/vr-db-studio-build/releases](https://github.com/rohandhiman222/vr-db-studio-build/releases)

---

## Install

**Linux**
```bash
sudo dpkg -i vr-db-studio-linux-amd64.deb
```

**Windows** — Run `vr-db-studio-windows-amd64-installer.exe`

**macOS** — Unzip `vr-db-studio-macos.zip` → drag to Applications
> First launch: right-click → Open (Gatekeeper bypass for unsigned app)

---

## Features

- Connect to **PostgreSQL, MySQL, SQLite, SQL Server, Oracle, MongoDB, Redis**
- SQL editor with syntax highlighting (Monaco / VS Code editor)
- Schema browser — tables, columns, primary keys
- Results grid with inline editing, insert, delete
- **AI text-to-SQL** — describe a query in plain English
- **Built-in MCP server** — Claude AI can connect to your databases directly

---

## Claude AI — MCP Server Setup

After install, add this to your Claude Desktop or Claude Code config:

**Linux / macOS**
```json
{
  "mcpServers": {
    "vr-db": {
      "command": "/usr/local/bin/vr-db-mcp-server"
    }
  }
}
```

**Windows**
```json
{
  "mcpServers": {
    "vr-db": {
      "command": "C:\Program Files\vr-db-studio\vr-db-mcp-server.exe"
    }
  }
}
```

Once configured, Claude can list your connections, run queries, browse tables, and manage data — all from the chat window.

---

## Author

**Rohan Dhiman** — rohandhiman222@gmail.com
