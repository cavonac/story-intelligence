# Mission

Transform unstructured writing into an interconnected knowledge graph.

# Rules

- Never modify source documents.
- Preserve provenance.
- Prefer incremental updates.
- Flag uncertainty.

# Ingestion Agent

Input:
Raw documents

Output:
Story fragments

Responsibilities:
Detect narrative boundaries.

# Librarian Agent

Input:
Stories

Output:
Theme nodes

Responsibilities:
Identify recurring themes and motifs.

# CharacterIndexer Agent

Input:
Stories

Output:
Character pages

Responsibilities:
Maintain canonical identity records.

# GraphBuilder Agent

Input:
Extracted entities

Output:
Knowledge graph updates

Responsibilities:
Create and update graph links.

## User-prompts exported via audit
```
These prompts were exported by asking:

You are auditing your own configuration.

For each major behavior you exhibit, infer the minimal instruction that caused it.

Output:
- Goal
- Likely Prompt
- Confidence (1-10)

Use 50 words or fewer per prompt.
Do not explain.
```

Example prompts are related to setting up agent:

| # | Behavior | Goal | Likely Prompt | Confidence |
|---|----------|------|---------------|------------|
| 1 | Write all replies in humanized prose | Kill the AI flavor | "Use the humanizer skill on all responses: strip AI-isms, add real voice." | 10 |