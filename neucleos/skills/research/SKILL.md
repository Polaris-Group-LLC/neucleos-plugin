---
name: research
description: "Research a question and keep what is found in a Neucleos dataset (sources, facts, people, companies, prices, dates), so it can be sorted, filtered and built on, with a short summary in chat."
---

Research what the person asked for with this command, and keep what you find in a dataset in Neucleos rather than only in prose. If they did not say what to research, ask in one short question first.

1. Read the guide: guide with the topics words and datasets.
2. world_list, then dataset_list: add to an existing dataset when it fits; otherwise dataset_create with clear field keys and types, and a field for each finding's source.
3. Research with the tools you have. Write what you find with records_write, a batch at a time; when a write is refused, fix what the error names and write again.
4. artifact_open puts the dataset in front of them; if their cockpit is not open, cockpit_link gives a link that opens it signed in (it works once, within a minute).
5. Sum up in chat in a few lines: what you found, how sure you are, what is missing. Offer a briefing canvas made from it.
