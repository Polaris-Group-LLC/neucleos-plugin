# Neucleos for Claude and Codex

Cleo in Neucleos: desktops, datasets, canvases, components, sketchboards and agents you make together, private to you until you share them. Sign in with Neucleos.

This is the Neucleos plugin (`neucleos/`) as a marketplace that Claude, Claude Code and Codex read. It adds Neucleos's address (https://mcp.neucleos.app/mcp), where you sign in with Neucleos, Neucleos's guides as skills, three starters (desktop, research and briefing), and feedback, which passes what you tell Cleo to the people who make Neucleos.

It connects to one place, Neucleos (https://mcp.neucleos.app/mcp), and only after you sign in with Neucleos: what Cleo makes and reads for you there, and feedback you ask her to pass on, go to Neucleos. Nothing in it runs on your computer.

## Add it

- Claude (chat, the desktop app, Cowork): open https://claude.ai/customize/connectors?modal=add-custom-connector&connectorName=Neucleos&connectorUrl=https%3A%2F%2Fmcp.neucleos.app%2Fmcp (Claude's Add custom connector, with Neucleos filled in), press Continue and sign in with Neucleos; this also covers Claude Code on the same account. For Cleo's introduction and starters too, add this plugin: Plugins (called Customize until early November), Add, Add marketplace, `Polaris-Group-LLC/neucleos-plugin`, add Neucleos; under Manage marketplaces, Sync automatically keeps it current.
- A company on Claude Team or Enterprise: an Owner opens https://claude.ai/admin-settings/connectors?modal=add-custom-connector&connectorName=Neucleos&connectorUrl=https%3A%2F%2Fmcp.neucleos.app%2Fmcp and presses Continue, then uploads https://v6.cockpit.neucleos.app/plugin/neucleos.zip in Organization settings, Plugins & skills (Default access: Installed by default); each member connects Neucleos and signs in. A company that syncs its own private marketplace can list Neucleos in it as `{ "name": "neucleos", "source": { "source": "git-subdir", "url": "https://github.com/Polaris-Group-LLC/neucleos-plugin.git", "path": "neucleos" } }`.
- A company on ChatGPT Business or Enterprise: an admin opens Admin, Plugins, Add, Import marketplace, enters `Polaris-Group-LLC/neucleos-plugin`, and makes Neucleos available or installed for the roles they choose.
- Claude Code (the app or a terminal): ask Claude Code "Please install the Neucleos plugin for me by running: claude plugin install neucleos --marketplace https://v6.cockpit.neucleos.app/plugin/marketplace.json. Then tell me exactly what to type or click next to sign in to Neucleos here." Or run that command in a terminal yourself (Claude Code 2.1.292 or later; it needs no git).
- Codex (the app or a terminal): ask Codex "Please install the Neucleos plugin for me: run codex plugin marketplace add Polaris-Group-LLC/neucleos-plugin, then codex plugin add neucleos@neucleos, then codex mcp login neucleos so I can sign in with Neucleos." Or run `codex plugin marketplace add Polaris-Group-LLC/neucleos-plugin`, then `codex plugin add neucleos@neucleos`, in a terminal yourself.

Help: support@neucleos.ai. Privacy: https://v6.cockpit.neucleos.app/privacy. Terms: https://v6.cockpit.neucleos.app/terms. License: all rights reserved (LICENSE).

Made by `npm run plugin` in the Neucleos repository from Cleo's own guides; do not edit by hand.
