# Neucleos

Cleo in Neucleos, for Claude (chat, Cowork and Claude Code) and Codex. It adds Neucleos's address (https://mcp.neucleos.app/mcp), where you sign in with Neucleos, Neucleos's guides as skills, three starters (desktop, research and briefing), and feedback, which passes what you tell Cleo to the people who make Neucleos.

It connects to one place, Neucleos (https://mcp.neucleos.app/mcp), and only after you sign in with Neucleos: what Cleo makes and reads for you there, and feedback you ask her to pass on, go to Neucleos. Nothing in it runs on your computer.

- Claude (chat, the desktop app, Cowork): Customize, Plugins, Add, Add marketplace, enter `Polaris-Group-LLC/neucleos-plugin` and add Neucleos from it (or download https://v6.cockpit.neucleos.app/plugin/neucleos.zip and choose Upload plugin); then on the plugin's Connectors tab add Neucleos and connect it.
- A company on Claude Team or Enterprise: an Owner uploads https://v6.cockpit.neucleos.app/plugin/neucleos.zip in Organization settings, Plugins & skills (Default access: Installed by default), or lists it in the company's own synced marketplace as `{ "name": "neucleos", "source": { "source": "git-subdir", "url": "https://github.com/Polaris-Group-LLC/neucleos-plugin.git", "path": "neucleos" } }`, and adds Neucleos's address in Organization settings, Connectors; each member connects it.
- Claude Code (the app or a terminal): ask Claude Code "Please install the Neucleos plugin for me: run claude plugin marketplace add Polaris-Group-LLC/neucleos-plugin, then claude plugin install neucleos@neucleos. When it's done, tell me how to load it and sign in to Neucleos here." Or run `claude plugin marketplace add Polaris-Group-LLC/neucleos-plugin`, then `claude plugin install neucleos@neucleos`, in a terminal yourself.
- Codex (the app or a terminal): ask Codex "Please install the Neucleos plugin for me: run codex plugin marketplace add Polaris-Group-LLC/neucleos-plugin, then codex plugin add neucleos@neucleos, then codex mcp login neucleos so I can sign in with Neucleos." Or run `codex plugin marketplace add Polaris-Group-LLC/neucleos-plugin`, then `codex plugin add neucleos@neucleos`, in a terminal yourself.

Help: support@neucleos.ai. Privacy: https://v6.cockpit.neucleos.app/privacy. License: all rights reserved (LICENSE).

Made by `npm run plugin` in the Neucleos repository from Cleo's own guides; do not edit it by hand.
