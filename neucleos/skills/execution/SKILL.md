---
name: execution
description: "Neucleos cloud execution: bounded Daytona jobs for code, rendering and Blender, with private outputs, progress and cancellation. Read before submitting or managing a cloud job."
---

# execution

Cloud execution runs code in a short-lived Daytona worker even when this chat has no shell. Call execution_capabilities for the World first. Only runtimes reported ready are available. Submit source files, an entrypoint, up to four output paths under out/, a title and a unique idempotency key with execution_submit. Python and Blender entrypoints end in .py; Node and browser entrypoints end in .js, .mjs or .cjs. Files live under /opt/neucleos/job, the working directory. Run at most 120 seconds. The pilot permits two concurrent jobs and twelve jobs per hour in an enabled World. Poll execution_read or execution_list for status, errors and outputs; execution_cancel stops an unwanted job. execution_download returns a five-minute download URL for one completed output. Jobs and results are private to the person who submitted them. A .blend is the editable scene; a .glb is a model for canvas viewing. Download links are attachments, not published apps or approved widget bundles. Keep using component_save for catalog components. Do not send account credentials into a job. GPUs and live remote desktop sessions are not enabled by these tools.
