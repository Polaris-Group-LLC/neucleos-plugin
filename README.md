# Neucleos for Claude and Codex

Work with Cleo in Neucleos: shared desktops and pages, live tables, client records, source-backed discovery, editable Designs, widgets and agents. New work stays private until you share it. Sign in with Neucleos.

This is the Neucleos plugin (`neucleos/`) as a marketplace that Claude, Claude Code and Codex read. It adds Neucleos's address (https://mcp.neucleos.app/mcp), where you sign in with Neucleos, Neucleos's guides as skills, starters (a desktop, research, a briefing, notes from a call, building a brand, and making things on-brand), and feedback, which passes what you tell Cleo to the people who make Neucleos.

It connects to one place, Neucleos (https://mcp.neucleos.app/mcp), and only after you sign in with Neucleos: what Cleo makes and reads for you there, and feedback you ask her to pass on, go to Neucleos. Nothing in it runs on your computer.

## Add it

- Supported Neucleos user sessions are Mac desktop apps and web browsers. CLI sessions are not supported.
- Claude on Mac or in a browser: add the Neucleos plugin from your organization's marketplace or the Polaris-Group-LLC/neucleos-plugin marketplace, or upload https://v6.cockpit.neucleos.app/plugin/neucleos.zip where plugin upload is available. Open its Connectors settings, connect Neucleos and sign in.
- ChatGPT on Mac or in a browser, and Codex mode in the Mac app: install the Neucleos plugin where it is available in your plugin directory or workspace, then use its Connect control and sign in. For a private test connection, use Add custom MCP server in the plugin settings with https://mcp.neucleos.app/mcp.
- After installing or updating, start a new conversation. Say “Cleo, open Neucleos.” In a Mac app, Neucleos should open in that app's built-in browser; in a web chat, it should open in another tab of the same browser. Use Chrome split view to see both together. If already open, reuse the correct tab.
- An organization can distribute the same package through its supported plugin administration controls. Availability and sign-in should be checked in the actual host; do not assume a connection made in another environment has transferred.

Help: support@neucleos.ai. Privacy: https://v6.cockpit.neucleos.app/privacy. Terms: https://v6.cockpit.neucleos.app/terms. License: all rights reserved (LICENSE).

Made by `npm run plugin` in the Neucleos repository from Cleo's own guides; do not edit by hand.
