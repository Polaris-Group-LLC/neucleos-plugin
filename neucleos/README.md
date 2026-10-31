# Neucleos

Cleo in Neucleos, for Claude (chat, Cowork and Claude Code) and Codex. It adds Neucleos's address (https://mcp.neucleos.app/mcp), where you sign in with Neucleos, Neucleos's guides as skills, and three starters: desktop, research and briefing.

- Claude (chat, the desktop app, Cowork): Customize, Plugins, Add, Add marketplace, enter `Polaris-Group-LLC/neucleos-plugin` and add Neucleos from it (or download https://v6.cockpit.neucleos.app/plugin/neucleos.zip and choose Upload plugin); then on the plugin's Connectors tab add Neucleos and connect it.
- A company on Claude Team or Enterprise: an Owner uploads https://v6.cockpit.neucleos.app/plugin/neucleos.zip in Organization settings, Plugins & skills (Default access: Installed by default), or lists it in the company's own synced marketplace as `{ "name": "neucleos", "source": { "source": "git-subdir", "url": "https://github.com/Polaris-Group-LLC/neucleos-plugin.git", "path": "neucleos" } }`, and adds Neucleos's address in Organization settings, Connectors; each member connects it.
- Claude Code: `claude plugin marketplace add Polaris-Group-LLC/neucleos-plugin`, then `claude plugin install neucleos@neucleos` (or `/plugin install neucleos@neucleos`).
- Codex: `codex plugin marketplace add Polaris-Group-LLC/neucleos-plugin`, then `codex plugin add neucleos@neucleos`.

Made by `npm run plugin` in the Neucleos repository from Cleo's own guides; do not edit it by hand.
