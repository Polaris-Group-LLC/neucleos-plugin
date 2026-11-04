---
name: opening
description: "When the user addresses you as Cleo or asks to open/use the Neucleos app or workspace, follow this skill. Reuse or open Neucleos inside the current Mac app or in another tab of the current web browser. Do not activate for unrelated conversation."
---

# opening

Activate this workflow when the person addresses you as Cleo, asks to open the Neucleos app or workspace, or explicitly asks to work in Neucleos. Merely installing the plugin does not turn ordinary conversations into Neucleos sessions. A question about the product is not by itself a request to open it.

Use the host context and browser tools already supplied by your session. Do not infer the host from the model name, OAuth client, or a general preferred-browser setting. Neucleos supports Mac apps and web browsers; a CLI is not a supported user experience.

1. Use the connected Neucleos tools. If the host asks to connect or authorize Neucleos, let the person finish that secure sign-in/consent flow, then resume. Never ask for passwords or verification codes in chat. Inspect the available tabs and reuse the Neucleos tab in the correct host when it is already open. Otherwise call cockpit_link for the requested World/artifact, or without arguments for the workspace. The production workspace is https://v6.cockpit.neucleos.app/.
2. In a native Mac app, open the link in that same app's built-in browser tab, beside this conversation. Do not try Chrome first or silently launch an external browser. This applies to both ChatGPT and Codex modes of the Mac app and to the Claude Mac app.
3. When this conversation is in a web browser, open the link in a new tab of that same browser. Tell the person it opens in a new tab. In Chrome, suggest its split-tab view so this conversation and Neucleos can be seen together. Do not claim split view was arranged unless it actually was.
4. Check the resulting page and say where it opened. Returning a link, submitting a navigation, or receiving artifact_open.opened is not proof that the browser displayed it. Reuse its existing browser sign-in. The MCP connection's authorization and the browser's session are separate; if the page requests sign-in, let the person complete it there and then resume. Only a link explicitly returned with signsIn:true establishes a sign-in handoff; never assume every link signs them in. Use world_list to confirm the connected account and available Worlds; a different browser sign-in may need the person's attention.
5. If the host provides no usable tab-opening capability, give the link and explain that the person must open it. Do not claim completion or substitute a different browser without their request. Only ask which host they use if the session context genuinely does not establish it.

After the workspace is available, continue the requested work through Neucleos's MCP tools with the person's access. Do not repeat setup in the same conversation. Respect an explicit request to keep Neucleos closed or use another destination.
