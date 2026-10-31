---
name: words
description: "Neucleos's words: Worlds, artifacts and their kinds, tabs and the deck, and opening the person's cockpit. Read before working in Neucleos for the first time in a conversation."
---

# words

- A World is a tenant (a person's own, or a company they belong to). Everything belongs to one World. world_list gives their Worlds (the first is their home World) and how many people are in each; world_members says who they are. Its owner (the founder) and admins invite people on the World page; you never invite, remove or accept anyone.
- People read other names in their cockpit than your tools use: a dataset is a Table (its records are rows, its fields columns), a canvas is a Page, a sketchboard is a Whiteboard, a component is a Widget, media are Files, write and show are Documents and Presentations, and a World's founder is its Owner. Say the names they read; your tools keep theirs.
- An artifact is a saved thing made in Neucleos. Kinds: write and show (Office documents and decks), dataset (a table; a sheet is a dataset), canvas (a page of text, media, components and datasets, on live data), media (an image, video or audio file), component (compiled, reusable React code in the World's catalog: a tab of its own, a thing on a desktop or a canvas, or a building block other components import), app (one self-contained HTML page), desktop (a surface of things you and the person use together), sketchboard (a whiteboard of shapes, arrows and notes, hand-drawn by default), song (lyrics and a style written together, to make into music).
- A dataset is durable structured data: records with described fields (text, number, date, boolean, url, choice, reference). No table is ever created for it. Records are addressed by _id; their values by field key.
- You never delete anything. A person deletes what they made in their cockpit (the bin on its tab): it waits 30 days in Recently deleted, on the right, where they can restore it, and then it is gone. A deleted thing is not in your lists and cannot be opened.
- A tab is an open artifact in the person's cockpit; their deck is the set of tabs open in a World. artifact_open puts one in front when their cockpit is open; when it is not, cockpit_link gives a link that opens it signed in, once, within a minute (its description says how to open it where you are, and what to tell them).
