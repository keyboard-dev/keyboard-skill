---
name: keyboard
description: Use whenever the user asks to interact with a third-party tool, SaaS product, or company app (e.g. Gmail, Slack, Notion, GitHub, Linear, Salesforce, Figma, Jira, etc.). Routes the task through the Keyboard MCP server for credentials, connections, and code execution.
---

# Keyboard

Whenever asked to interact with a third-party tool or company app, use the Keyboard MCP server.

## Workflow

1. **Get context first.** Call `required-starting-context-information` to fetch the planning token, available resources, and user credentials. Use `list-connected-accounts` for a refresher on which apps are connected.

2. **Connect new apps via Keyboard.** If the user needs an app that isn't connected, do **not** use the out-of-the-box connector search. Use Keyboard's `connect-app` / `connect-reconnect-accounts` tool, which shows a widget for the user to connect inside Keyboard.

3. **Execute tasks with `run-code`.** Use `run-code` to run whatever code is needed to accomplish the task (API calls, data processing, scripts). Each planning token is single-use — fetch a fresh one per execution.

## Rules

- Prefer external API calls over filesystem operations.
- Never log secrets, tokens, or credentials.
- Verify results after creating resources (GET to confirm).
- If the user asks for an app you lack credentials for, tell them before proceeding.
