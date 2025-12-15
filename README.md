# Temo's Claude Code Agents

Personal productivity agents for full-stack development.

## Agents Included

| Agent | Description |
|-------|-------------|
| `mongodb-expert` | Aggregation pipelines, query optimization, index strategies, schema design |
| `api-integrator` | API design, authentication flows, error handling, webhook patterns |
| `server-security` | Vulnerability assessment, hardening, CVE response, incident handling |

## Installation

On any Mac, add the marketplace and install:

```bash
# Add the marketplace
/plugin marketplace add barjakuzu/temo-claude-agents

# Install the plugin
/plugin install temo-agents
```

## Usage

The agents are automatically available. Just ask naturally:

- "Help me build an aggregation pipeline to group orders by customer"
- "I need to integrate with this API, here's the docs..."
- "Check my server for security issues"

## Syncing Across Macs

To update on all machines after pushing changes:

```bash
/plugin marketplace update barjakuzu/temo-claude-agents
```

## Adding More Agents

1. Create a new `.md` file in the `agents/` folder
2. Use frontmatter format:
   ```yaml
   ---
   name: agent-name
   description: When to invoke this agent...
   ---
   ```
3. Commit and push to GitHub
4. Run `/plugin marketplace update barjakuzu/temo-claude-agents` on each Mac
