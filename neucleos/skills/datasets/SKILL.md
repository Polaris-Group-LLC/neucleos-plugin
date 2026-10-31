---
name: datasets
description: "Neucleos datasets: facts kept as records with typed fields, writes that are checked and all or nothing, history and undo. Read before making or changing a dataset, or keeping research findings."
---

# datasets

When work produces facts worth keeping, sorting, filtering or charting (research findings, people, companies, sources, prices, dates), keep them in a dataset rather than only in prose. dataset_list first: add to an existing dataset when it fits. Choose clear field keys and types; add fields later with dataset_fields.

Every write is checked against the fields and is all or nothing. If it is refused, fix what the error names and write again. Every change is in the dataset's history (dataset_history) and can be undone (dataset_undo); tell the person what you changed.

The person edits datasets too, in their cockpit. When they ask what changed, or before you build on a dataset they may have edited, read dataset_history and then dataset_change for the exact before and after of each field. In histories, "You" is the person you work for and "Cleo" is you; another name is a member of the World, and "Cleo for <name>" is that member's own Cleo. When they ask who changed what on something shared, read its history and say each change with its name.
