# Pinnu for Claude

Pinnu is a notes app in the spirit of Google Keep: notes and checklists pinned to a board, on
the web at https://pinnu.app and on Android and iPhone. This plugin connects Claude to your
Pinnu notes through Pinnu's MCP server at https://pinnu.app/mcp.

Notes are plain Markdown, so Claude reads many notes in one call and changes them a piece at a
time, like editing a file. Checklists are Markdown task lists, so Claude can tick items off.
Everything Claude changes is marked with its name in the app and kept in the note's history for
30 days, so you can undo it with one tap.

## What you can ask

- "Make a packing list for a weekend in the mountains in Pinnu."
- "Read my notes labelled Work and sum up the week."
- "Tick milk and bread on the shopping list."
- "Add today's meeting notes to my log and remind me on Friday at 9."
- "What does the receipt in my Expenses note say?" (Claude can look at attached pictures and PDFs.)

## Install in Claude Code

```
/plugin marketplace add softgot/pinnu-plugin
/plugin install pinnu@pinnu
```

Then run `/mcp`, choose `pinnu` and sign in with your Pinnu account. You approve the
connection on pinnu.app, and Claude can then reach only your notes. You can disconnect it in
the app under Account → Connect AI.

## Privacy

Claude reaches your notes only after you approve it. Notes you lock in the app are never shown
to Claude, and sharing or publishing a note always needs your approval in the app. See https://pinnu.app/integritet for the
privacy policy and https://pinnu.app/villkor for the terms. Contact: contact@pinnu.app.
