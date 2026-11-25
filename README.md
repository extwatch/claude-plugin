# Ext Watch plugin for Claude Code

Ext Watch tracks the Chrome Web Store every day. This plugin connects Claude Code to the Ext Watch MCP server at `https://app.extwatch.com/api/mcp`, so you can research Chrome extensions from your terminal: search the store, compare competitors, follow publishers, see new launches and listing changes, find rising extensions and read what users say in reviews.

All data comes from Ext Watch's own crawl. The tools are read-only.

## Requirements

- Claude Code with plugin support.
- An Ext Watch account on the **Pro** or **Scale** plan. AI apps are unavailable on other plans. See https://extwatch.com/ai-apps/plans.

## Install

In Claude Code, run:

```
/plugin marketplace add earlygap/extwatch-claude-plugin
/plugin install extwatch@extwatch
```

Then run `/mcp`, pick `extwatch` and sign in with your Ext Watch account. Sign-in uses OAuth in your browser. The plugin stores no keys or secrets.

## What's included

- `.mcp.json`: the remote Ext Watch MCP server (HTTP).
- `skills/chrome-extension-research`: tells Claude when the Ext Watch tools fit a question and how to report their results.

## Example questions

- "Which ad blockers launched this month?"
- "Compare the top three tab managers."
- "What do users complain about in reviews of grammar checkers?"

## Data and privacy

Requests go only to `app.extwatch.com`. See the privacy policy at https://extwatch.com/privacy.

## Support

https://extwatch.com/support

## License

MIT. See [LICENSE](LICENSE).
