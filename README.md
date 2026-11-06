# Neucleos for Claude and Codex

Work with Cleo in Neucleos: shared desktops and pages, live tables, client records, source-backed discovery, editable Designs, widgets and agents. New work stays private until you share it. Sign in with Neucleos.

This is the Neucleos plugin (`neucleos/`) as a marketplace that Claude, Claude Code and Codex read. It adds Neucleos's address (https://mcp.neucleos.app/mcp), where you sign in with Neucleos, Neucleos's guides as skills, starters (a desktop, research, a briefing, notes from a call, building a brand, and making things on-brand), and feedback, which passes what you tell Cleo to the people who make Neucleos.

It connects to one place, Neucleos (https://mcp.neucleos.app/mcp), and only after you sign in with Neucleos: what Cleo makes and reads for you there, and feedback you ask her to pass on, go to Neucleos. Nothing in it runs on your computer.

## Add it

- Supported Neucleos user sessions are Mac desktop apps and web browsers. CLI sessions are not supported.
- Claude on Mac or in a browser: add the Neucleos plugin from your organization's marketplace or the Polaris-Group-LLC/neucleos-plugin marketplace, or upload https://v6.neucleos.app/plugin/neucleos.zip where plugin upload is available. Open its Connectors settings, connect Neucleos and sign in.
- ChatGPT on Mac or in a browser, and Codex mode in the Mac app: install the Neucleos plugin where it is available in your plugin directory or workspace, then use its Connect control and sign in. For a private test connection, use Add custom MCP server in the plugin settings with https://mcp.neucleos.app/mcp.
- After installing or updating, start a new conversation. Say “Cleo, open Neucleos.” Cleo checks where you are viewing the chat now, then reuses the correct Neucleos tab there. In a Mac app, it opens in that app's built-in browser; in a web chat, it uses the same web browser even if a desktop app is also connected. If the current surface is unclear, Cleo asks once and provides the link. It verifies the page and visibility before saying it opened. If Cleo cannot arrange Chrome split view, right-click its Open Neucleos link and choose “Open link in split view”. If Neucleos is already open, keep the chat tab active, right-click the Neucleos tab and choose “New split view with current tab”. No additional browser extension is required.
- An organization can distribute the same package through its supported plugin administration controls. Availability and sign-in should be checked in the actual host; do not assume a connection made in another environment has transferred.

Help: support@neucleos.ai. Privacy: https://v6.neucleos.app/privacy. Terms: https://v6.neucleos.app/terms. License: all rights reserved (LICENSE).

Made by `npm run plugin` in the Neucleos repository from Cleo's own guides; do not edit by hand.
