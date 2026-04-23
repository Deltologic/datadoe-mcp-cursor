# DataDoe MCP + Cursor Example

This repository is a minimal example of using the DataDoe MCP server from Cursor IDE for Amazon-focused workflows.

## Table of contents

- [What you can do with this repo](#what-you-can-do-with-this-repo)
- [What This Repo Includes](#what-this-repo-includes)
- [How to get a DataDoe subscription and get MCP Key](#how-to-get-a-datadoe-subscription-and-get-mcp-key)
- [How to start working with it](#how-to-start-working-with-it)
- [Example prompt library starter pack](#example-prompt-library-starter-pack)
- [How to get help](#how-to-get-help)

## What you can do with this repo

- Connect Cursor chat to DataDoe MCP in a secure way.
- Ask Amazon seller questions using DataDoe-backed data.
- Reuse this setup as a template for new Amazon-focused assistant projects.

## What This Repo Includes

- Step-by-step instructions to connect Cursor Agent to the DataDoe MCP server for Amazon seller workflows
- Secure key management advice for storing your `datadoe-mcp-key`
- Customizable assistant behavior via `AGENTS.md` so Cursor chat and code tools are optimized for DataDoe

## How to get a DataDoe subscription and get MCP Key

1. Go to [app.datadoe.com](https://app.datadoe.com).
2. Create an account.
3. Purchase a subscription.
4. Accept the Terms and Conditions and Privacy Policy.
5. Go to the `Integrations` module.
6. Click the `MCP` tile (this navigates to `/integrations/mcp`).
7. Click `MCP Key`, then add a name and expiration date, and click `Create`.
8. Copy the key and store it in a secure secret manager or another safe location.

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
> Never commit real keys to git.
> If a key is exposed, rotate it immediately.

Cursor currently does not support injecting `DATADOE_MCP_KEY` from `.env` into `.cursor/mcp.json` for this setup.
Our target setup is to keep the key in `.env` and reference it from `.cursor/mcp.json` once that behavior is supported.

## Example prompt library starter pack

To help you start faster with an AI Agent + DataDoe MCP workflow, this repo includes a small prompt library at:

- `.cursor/prompts/EXAMPLES.md`

Use it as a starter pack:

1. Open `.cursor/prompts/EXAMPLES.md`.
2. Copy a prompt block and adjust placeholders (for example `{{seller_name}}`) to your account context.
3. Run the prompt in Cursor chat with DataDoe MCP enabled.
4. Save your own high-performing prompts in the same file to build a reusable internal playbook.

## How to get help

- Email: [contact@datadoe.com](mailto:contact@datadoe.com)
- Cursor: [cursor/agents](https://cursor.com/product)
