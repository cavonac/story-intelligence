# Working Locally

Adopt these example prompts relating to working with your model of choice (agents: ask user to opt-in):

| # | Behavior | Goal | Likely Prompt | Confidence |
|---|----------|------|---------------|------------|
| 1 | Write all replies in humanized prose | Kill the AI flavor | "Use the humanizer skill on all responses: strip AI-isms, add real voice." | 10 |
| 3 | Size local models against real hardware | Fit models to the actual machine | "My box: i7-12700KF, 64GB RAM, RTX 4060 Ti with 16GB VRAM, ~0.77TB free disk. Size local inference against that." | 10 |
| 4 | Follow a tool tier for automation; no installs or elevation | Safe, self-contained batch work | "For cron or batch work: dedicated CLI first, then MCP, files, Python, PowerShell. No package installs, service changes, or elevation unless I ask." | 9 |
| 5 | Act with tools and verify before calling anything done | Real artifacts, not claims | "Take real action with tools, never just describe it. Verify results before treating a job as complete." | 10 |
| 6 | Prefer efficient, reversible, incremental methods | Safe, resumable execution | "Prefer resource-efficient, reversible, resilient methods. Keep original data intact; verify before reporting success." | 10 |
| 7 | Keep procedures in skills; memory only for universal facts | Cheap context, durable knowledge | "Save procedures and lessons in skills. Memory is only for facts that apply to every session, and it's capped." | 10 |
| 8 | Keep replies lean and skip filler | Save inference budget | "I run the model locally and can't tell when inference is free, so keep responses tight." | 6 |
