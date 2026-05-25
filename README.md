# Zernio for Claude Code

Schedule, publish, and analyze social media across 15+ platforms (Instagram, TikTok, YouTube, X, LinkedIn, Facebook, Threads, Pinterest, Reddit, Bluesky, WhatsApp, Telegram, Snapchat, Google Business) directly from Claude Code, plus a unified inbox, paid-ads management, and analytics. Powered by Zernio's hosted MCP server (300+ tools).

## Install

```
/plugin marketplace add zernio-dev/zernio-claude-plugin
/plugin install zernio@zernio
```

When you enable the plugin, Claude Code prompts for your **Zernio API key**. Create one at [zernio.com/dashboard/api-keys](https://zernio.com/dashboard/api-keys) (it starts with `sk_`). The key is stored in your system keychain, never in plaintext.

## What you can do

- "List my connected social accounts" (`/zernio:accounts`)
- "Schedule a LinkedIn post for tomorrow at 9am: ..."
- "Cross-post this to X, LinkedIn, and Bluesky right now"
- "Show my unread Instagram DMs"
- "What's the best time to post this week?"
- "List my active Meta ad campaigns and their spend"

## How it works

This plugin bundles a single remote MCP server, `https://mcp.zernio.com/mcp` (Streamable HTTP), authenticated with your API key via the `Authorization: Bearer` header. No local install or Python required.

> Note: the API-key method is used here because Claude Code plugins can't run a browser OAuth flow. (The Claude.ai / Claude Desktop connector uses OAuth instead.)

## Links

- Docs: https://docs.zernio.com/resources/mcp
- Dashboard: https://zernio.com/dashboard
- Support: support@zernio.com
