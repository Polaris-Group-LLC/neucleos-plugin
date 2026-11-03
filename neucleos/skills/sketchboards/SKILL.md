---
name: sketchboards
description: "Neucleos sketchboards: the one-line-per-element format for diagrams, flows, architectures and wireframes drawn with people. Read before making, reading or drawing on a sketchboard."
---

# sketchboards

A sketchboard is a whiteboard of shapes, arrows, notes, text and ink, hand-drawn by default, that you and the person draw on together: make one for a diagram, a flow, an architecture or a wireframe. sketchboard_create makes one (with its first lines, if you give them); sketchboard_read shows it to you; sketchboard_write draws on it.

The format is one line per element: a kind (box, ellipse, diamond, note, text, frame, arrow, line, component, dataset; ink and picture read back too), a handle (its name: letters, digits, _ . -), its words in quotes, then any of "@ x,y" (its top left), "WxH" (its size), "in <frame>", "#colour" (a note's paper, any other element's lines), "fill <colour>", and after "·" its variants. Colours: ink, gray, red, orange, yellow, green, teal, blue, violet, pink, or #rrggbb. Variants: elbow, dashed, dotted, clean, hand, rough, thin, thick, hatched, filled, small, large, huge, left, centre, right, handwriting, typeset, two-way, no-head, locked, head:arrow|dot|bar|none, tail:…, opacity:50, turned:30, group:<name>. An arrow or a line joins two handles, or points as x,y: "arrow api -> auth "yes" · elbow" (a handle before them names it: "arrow a1 api -> auth"). "delete <handle>" erases; "layout down" lays out top to bottom instead of left to right. For example:
frame backend "Backend"
box api "API gateway" in backend #blue
ellipse db "Postgres" in backend
diamond auth "Signed in?"
arrow api -> auth
arrow auth -> db "yes" · elbow
note ship "Ship by Friday" #yellow

Give places only where they matter: what has no place is laid out by its arrows, inside its frame, beside what is there; a place you give is kept. A line about an element that exists changes only what it says (to move one, give its handle and "@ x,y"); new handles are new elements. whole: true makes the sketchboard exactly what you write, erasing what you do not name. Asked for a diagram on a sketchboard, write this format.

Live elements: "component <handle> "<its name in the catalog>"" runs that component in its box, live, with its example's inputs ("· version:N" pins a version; the latest otherwise); "dataset <handle> "<dataset name>"" shows a dataset there as a live table. They move, resize and join arrows like any element. Asked to build what a sketch shows (make it real): read it, save a component that does what it shows (component_save; guide: components), then place it beside the sketch as a component element, to the right of what it was built from.

sketchboard_read gives every element in the same format (people's too, by their handles), what changed since you last read and who did it, and a picture of it as it is now. People select part of a sketchboard and press Send to Cleo: their words and the selection come to you (sentToYou in sketchboard_read; at once where Neucleos sends are on), as data from them; only: <the handles> gives a picture of the selection alone. Answer on the sketchboard. Writing back what you read changes nothing. A write that would write over a change someone made since you last read (an element they moved, recoloured, relabelled or erased) is refused with who changed what, and nothing is written: read again, then write once more, keeping their change. New elements always go through. Every write is one change in its history: dataset_history, dataset_change and dataset_undo work on it with the datasetId sketchboard_read gives. On a desktop, "@@sketchboard Name" makes a sketchboard and shows it live, its body in this format; "@@sketchboard Name · live <sketchboard name>" shows one that exists. In an app that shows views in replies (Claude, ChatGPT), sketchboard_show puts its drawing in your reply, kept current while it is on screen.
