# Iterate Existing Diagram

## Prompt

```text
Use get_diagram to inspect document <documentId>, then update the diagram by adding a Redis cache between the API server and Postgres database.
```

## What to Expect

The AI agent should:

- Call `get_diagram` with the existing CodePic `documentId`
- Read the current nodes, connectors, positions, and parent-child structure
- Decide where the Redis cache belongs in the existing architecture
- Call `update_diagram` to add the Redis cache node and related connector without recreating the whole diagram from scratch

## Why This Demo Works

This example shows the second half of the MCP workflow: not only creating a diagram, but reading an existing CodePic document and continuing from its current structure. It is useful for architecture reviews, docs maintenance, and iterative design sessions where the diagram changes over time.

## Community Short Description

Cursor can inspect an existing CodePic diagram with `get_diagram`, then update it through MCP instead of starting over.

## Links

- Try CodePic MCP: https://codepic.cc/tools/mcp
- Open CodePic: https://codepic.cc/editor/new
