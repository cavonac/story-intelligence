# Mission

Transform unstructured writing into an interconnected knowledge graph.

## Shared rules

- Never modify source documents.
- Preserve provenance for every fact added to the knowledge graph.
- Prefer incremental updates over rebuilding existing pages.
- Flag uncertainty rather than presenting an inference as fact.
- Follow the shared [Agent Rules](../rules/agent-rules.md).
- Follow each agent’s own instructions for its specific responsibilities.

## Agent catalog

### Character Agent

Instructions: [Character Agent](./character.md)

- **Input:** Stories
- **Output:** Character pages
- **Owns:** Canonical character identity records

### Ingestion Agent

Instructions: [Ingestion Agent](./ingestion.md)

- **Input:** Raw documents
- **Output:** Story fragments
- **Owns:** Detecting and recording narrative boundaries

### Historian Agent

Instructions: [Historian Agent](./historian.md)

- **Input:** Stories
- **Output:** History pages and timelines
- **Owns:** Canonical history and timeline records

### Lorekeeper Agent

Instructions: [Lorekeeper Agent](./lorekeeper.md)

- **Input:** Stories
- **Output:** Lore nodes
- **Owns:** Canonical records of the world’s lore

### Theme Analyst Agent

Instructions: [Theme Analyst Agent](./theme-analyst.md)

- **Input:** Wiki pages
- **Output:** Theme pages
- **Owns:** Identifying and documenting recurring ideas
