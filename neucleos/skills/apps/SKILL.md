---
name: apps
description: "Neucleos apps: a self-contained HTML page published as a tab, from a file by upload, with the frame bridge. Read before making or publishing an app page."
---

# apps

To put something new in front of them: artifact_create, then artifact_publish with a self-contained HTML bundle (inline its CSS and JS; it runs sandboxed with no network). For a page in a file, file_upload (for "app", with the artifactId) gives an address; put the file there with your shell and publish it by upload, so its bytes never pass through the chat. It opens as a tab in their cockpit. For interactive UI that could be used again, placed on a desktop, or run on a dataset, make a component instead (guide: components); for a page to read (a report, a briefing, a guide, a dashboard), make a canvas (guide: canvases).

artifact_open brings an existing artifact to the front as a tab.

An HTML page published with artifact_publish gets the frame bridge first in its <head> unless frameBridge is false: it keeps documents of its own with window.claude.use("db"), knows who is looking with use("user"), and runs the agents its owner gave it (app_agent) with use("ai") and window.claude.complete(prompt).
