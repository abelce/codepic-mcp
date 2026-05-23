# CodePic MCP Examples

Generate editable hand-drawn diagrams from Cursor, Claude Desktop, and other MCP clients.

CodePic MCP lets an AI coding agent create diagrams directly in CodePic instead of returning static images, Mermaid snippets, or JSON that you have to paste manually. The result opens in the CodePic editor, where you can still move shapes, edit labels, adjust connectors, share a read-only link, and export PNG or JSON.

## Quick Start

### Cursor

Create `.cursor/mcp.json` in your project:

```json
{
  "mcpServers": {
    "codepic": {
      "url": "https://codepic.cc/api/mcp/mcp",
      "headers": {
        "Authorization": "Bearer cpk_your_api_key_here"
      }
    }
  }
}
```

### Claude Desktop

Add CodePic to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "codepic": {
      "type": "streamableHttp",
      "url": "https://codepic.cc/api/mcp/mcp",
      "headers": {
        "Authorization": "Bearer cpk_your_api_key_here"
      }
    }
  }
}
```

Replace `cpk_your_api_key_here` with an API key from CodePic.

## Examples

| Example | What It Generates | Prompt |
|---|---|---|
| [System architecture](examples/system-architecture.md) | Next.js SaaS architecture diagram | Next.js + Supabase + Postgres + R2 + Stripe + Vercel |
| [Database ER diagram](examples/database-er-diagram.md) | SaaS billing data model | Users, teams, subscriptions, invoices, payments |
| [OAuth sequence flow](examples/oauth-sequence-flow.md) | PKCE login sequence diagram | Browser, app server, identity provider, database |
| [CI/CD pipeline](examples/cicd-pipeline.md) | GitHub Actions deployment pipeline | Type-check, lint, build, preview, production |
| [Data pipeline](examples/data-pipeline.md) | Analytics pipeline diagram | Segment, Snowflake, dbt, Metabase |

## Useful Links

- CodePic: https://codepic.cc
- MCP guide: https://codepic.cc/tools/mcp
- ER diagram maker: https://codepic.cc/tools/er-diagram-maker
- Flowchart maker: https://codepic.cc/tools/flowchart-maker
- Wireframe tool: https://codepic.cc/tools/wireframe-tool

## Community Post Angle

If you share this project, lead with the workflow:

> I connected Cursor to a diagram editor through MCP, so it can generate editable architecture diagrams instead of Mermaid text.

Avoid generic product claims like "best diagram tool". Developer communities respond better to a concrete workflow and real examples.

