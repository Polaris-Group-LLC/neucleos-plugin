---
name: datasets
description: "Neucleos datasets: facts kept as records with typed fields, writes that are checked and all or nothing, history and undo. Read before making or changing a dataset, or keeping research findings."
---

# datasets

For client, account, prospect or deal discovery, read the clients guide first: use records, work, sources and claims. For other facts worth keeping, sorting, filtering or charting (research findings, prices, dates), keep them in a dataset rather than only in prose. dataset_list first: add to an existing dataset when it fits. Choose clear field keys and types; add fields later with dataset_fields. To show reverse links or dependencies on each row, add a related column with dataset_fields: type "related", related { datasetId: the relationship table, matchField: its reference back to this table, valueFields: the reference fields to follow }. Omit valueFields to show the matching relationship rows themselves. These columns are computed, read-only, and follow live records; never maintain a second list in text. records_query returns each related value as { items: [{ recordId, datasetId, artifactId, worldId, label }], state, message? }. No links recorded does not mean a dependency review is complete. Filtering and sorting apply to stored fields; filter the source table when inspecting relationships.

Every write is checked against the fields and is all or nothing. If it is refused, fix what the error names and write again. Every change is in the dataset's history (dataset_history) and can be undone (dataset_undo); tell the person what you changed.

The person edits datasets too, in their cockpit. When they ask what changed, or before you build on a dataset they may have edited, read dataset_history and then dataset_change for the exact before and after of each field. In histories, "You" is the person you work for and "Cleo" is you; another name is a member of the World, and "Cleo for <name>" is that member's own Cleo. When they ask who changed what on something shared, read its history and say each change with its name.
