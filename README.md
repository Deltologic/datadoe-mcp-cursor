# DataDoe MCP + Cursor Example

This repository is a minimal example of using the DataDoe MCP server from Cursor IDE for Amazon-focused workflows.

## Table of contents

- [What you can do with this repo](#what-you-can-do-with-this-repo)
- [What this repo is](#what-this-repo-is)
- [How to start working with it](#how-to-start-working-with-it)
- [How to get a DataDoe subscription](#how-to-get-a-datadoe-subscription)
- [How to get help](#how-to-get-help)
- [Recommended repository cleanup](#recommended-repository-cleanup)
- [Tags](#tags)

## What you can do with this repo

- Connect Cursor chat to DataDoe MCP in a secure way.
- Ask Amazon seller questions using DataDoe-backed data.
- Reuse this setup as a template for new Amazon-focused assistant projects.

## What this repo is

- A starter setup for connecting Cursor to DataDoe MCP.
- A reference for secure local API key configuration.
- A base project for asking Amazon selling questions through MCP in Cursor chat.

## How to start working with it

1. Clone the repository:
   ```bash
   git clone https://github.com/Deltologic/datadoe-mcp-cursor
   cd datadoe-mcp-cursor
   ```
2. Open `.cursor/mcp.json` and set your key directly in headers:
   - `"datadoe-mcp-key": "your_key_here"`
3. Restart Cursor (or reload window) so the updated MCP configuration is loaded.
4. Open Cursor chat and ask an Amazon-related question.

> [!CAUTION]
> Treat `DATADOE_MCP_KEY` like a password. Do not publish repositories, screenshots, or logs that contain this key.
> If a key is exposed, rotate it immediately.

Cursor currently does not support injecting `DATADOE_MCP_KEY` from `.env` into `.cursor/mcp.json` for this setup.
Our target setup is to keep the key in `.env` and reference it from `.cursor/mcp.json` once that behavior is supported.

## How to get a DataDoe subscription

- For subscription and access details, contact DataDoe support.
- Ask for MCP access and your `DATADOE_MCP_KEY`.

## How to get help

- Email: [contact@datadoe.com](mailto:contact@datadoe.com)

## Recommended repository cleanup

For each repository using this template, keep settings lean:

- Disable GitHub Wiki if not used.
- Disable GitHub Projects if not used.
- Disable Discussions if not used.
- Keep branch protection minimal but enabled for your main branch.
- Do not commit `.env` or real API keys.

## Tags

`DataDoe` `MCP` `Cursor` `Amazon` `Amazon Seller` `AI Assistant` `LLM` `Prompting`
