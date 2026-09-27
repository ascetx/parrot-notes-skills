# ParrotNotes Skills

Agent Skills for [ParrotNotes](https://parrotnotes.app), an AI note-taker for in-person meetings that records in the background with no meeting bot.

## Skills

| Skill | What it does |
|---|---|
| [`parrotnotes`](skills/parrotnotes) | Find, read, summarise and save insights for your ParrotNotes in-person meeting notes and written notes |

## Install

**Hermes Agent**

Add this repo as a skill tap, then install from it:

```bash
hermes skills tap add ascetx/parrot-notes-skills
hermes skills install ascetx/parrot-notes-skills/parrotnotes
```

Or install the skill directly without adding the tap:

```bash
hermes skills install ascetx/parrot-notes-skills/skills/parrotnotes
```

For the full integration, with the MCP server set up for you, install the Hermes plugin instead: [ascetx/parrot-notes-hermes-plugin](https://github.com/ascetx/parrot-notes-hermes-plugin).

**Claude Code, Codex, Cursor, Gemini CLI and other Agent Skills clients**

```bash
npx skills add ascetx/parrot-notes-skills
```

Add `-g` to install for your user rather than the current project, or `-a <agent>` to pick a client, for example `-a claude-code`.

## Requirements

These skills drive the ParrotNotes MCP connector. Installing a skill does not set up the connector, so add it to your client first.

- Endpoint: `https://mcp.parrotnotes.app/mcp`
- Transport: Streamable HTTP
- Auth: OAuth 2.0 with Dynamic Client Registration, no API key
- A ParrotNotes account. The free tier works.

Per-client setup: https://parrotnotes.app/docs/mcp

## Format

Built to the [Agent Skills](https://agentskills.io) open standard.

## Support

support@parrotnotes.app
