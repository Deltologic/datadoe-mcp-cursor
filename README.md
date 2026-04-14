# DataDoe MCP + Cursor Example

This repository is a minimal example of using the DataDoe MCP server from Cursor IDE for Amazon-focused workflows.

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
2. Create `.env` in the repo root:
   - `DATADOE_MCP_KEY=your_key_here`
3. Keep `.cursor/mcp.json` configured with:
   - `"datadoe-mcp-key": "${DATADOE_MCP_KEY}"`
4. Restart Cursor (or reload window) so environment variables are loaded.
5. Open Cursor chat and ask an Amazon-related question.

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
