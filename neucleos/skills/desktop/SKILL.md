---
name: desktop
description: "Start a Neucleos Desktop for what the person is working on: registered pieces they can use at once (text, a list, a table, a poll, a form) beside the chat, made with object_create and opened in their cockpit."
---

The person has requested Neucleos work. Follow the opening skill first if the workspace is not already open in this conversation.

Make the person a desktop in Neucleos for what they asked for with this command. If they did not say what it is for, ask in one short question first.

1. Read the guide: guide with the topics words and desktops.
2. world_list, and work in their home World unless they named another. Look before you make (search, artifact_list with kind desktop): reopen a desktop that already fits rather than make a near-duplicate.
3. desktop_create makes the Desktop; then object_create a few registered pieces (object_catalog lists them) and place them on it with object_update: a Text of what it is for, a List of next steps and a Table or Poll of what matters, not prose alone. desktop_write is the legacy block-format path and refuses an object-backed Desktop.
4. artifact_open puts it in front of them. If their cockpit is not open, use cockpit_link and the opening skill to open it in the current host, then verify it and say where it opened.
5. Tell them in two lines what is on it and what you could add next.
