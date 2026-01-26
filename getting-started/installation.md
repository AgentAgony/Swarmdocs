# Installation

Get Vexorbis up and running in minutes.

## Prerequisites

- **Docker** (recommended) or Python 3.11+
- An AI coding assistant that supports MCP:
  - Antigravity
  - Cursor
  - Claude Desktop
- API key for at least one LLM provider:
  - `GEMINI_API_KEY` (recommended)
  - `OPENAI_API_KEY` (fallback)

## Docker Installation (Recommended)

The fastest way to get started:

```bash
# Request access via the website
cd vexorbis

# Start the server
docker compose up -d --build
```

Verify it's running:
```bash
docker ps | grep vexorbis
# Should show: vexorbis-mcp-server
```

## Manual Installation

For development or customization:

```bash
# After receiving access, clone and setup
cd vexorbis

# Create virtual environment
python -m venv .venv
source .venv/bin/activate  # or .venv\Scripts\activate on Windows

# Install dependencies
pip install -e ".[dev]"

# Set your API key
export GEMINI_API_KEY="your-key-here"

# Run the server
python server.py
```

## IDE Configuration

Add Vexorbis to your IDE's MCP configuration.

### Antigravity

Edit `~/.antigravity/settings.json`:

```json
{
  "mcpServers": {
    "vexorbis-orchestrator": {
      "command": "docker",
      "args": ["exec", "-i", "vexorbis-mcp-server", "fastmcp", "run", "server.py"]
    }
  }
}
```

### Cursor

Edit `~/.cursor/mcp.json`:

```json
{
  "servers": {
    "vexorbis": {
      "command": "docker",
      "args": ["exec", "-i", "vexorbis-mcp-server", "fastmcp", "run", "server.py"]
    }
  }
}
```

## Verify Installation

In your IDE, try using the `search_codebase` tool:

```
Search for "authentication" in this project
```

If Vexorbis responds with code results, you're ready!

---

## Next Steps

- [Quick Start](./quickstart.md) — Run your first Vexorbis task
- [Configuration](../reference/configuration.md) — Customize Vexorbis's behavior
