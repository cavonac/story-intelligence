# Creative-Writing Wiki Migration

You are a Hermes agent working with local data. Follow the installed `llm-wiki` skill, including its Karpathy-inspired guidelines; don’t invent conventions.

Run only the phase(s) the user requests. If they ask for the full migration without naming phases, run phases 1–4. Keep destination setup separate from migration.

### 1. Inspect and plan
- Read the skill, then inspect the current wiki’s `SCHEMA.md`, `index.md`, and recent `log.md`, if present.
- Inventory likely creative-writing content: fiction, characters, settings, plots, drafts, worldbuilding, and related notes.
- Report the proposed scope and any ambiguous items. Keep the source wiki read-only.

### 2. Choose and prepare the destination
- Check accessible wiki locations for an existing, dedicated creative-writing wiki. Don’t treat a general wiki as the destination just because it contains writing notes.
- If one exists, use it and read its schema, index, and recent log.
- If none exists, this migration request authorizes creating a separate wiki using the skill’s setup conventions. Don’t overwrite an existing directory or change global configuration. If the destination path is unclear or unsafe, pause and ask.
- This phase may happen before or after inspection. Don’t migrate until the destination is ready.

### 3. Migrate
- Copy only the agreed creative-writing content. Never move, delete, or alter source files.
- Follow the skill’s rules for structure, provenance, links, index updates, and logging. Preserve distinct drafts and versions; don’t invent details or silently resolve contradictions.
- Reuse equivalent destination pages where appropriate. If a destination conflict requires overwriting or merging content, pause and ask.
- Don’t deduplicate or clean up legacy documents as part of the migration.

### 4. Verify and report
- Check migrated files, links, index, log, and applicable skill checks.
- Report the source and destination, what was copied or flagged, and any remaining decisions. Ask separately before cleanup or archiving.

### Future ingestion
- Route each new item to one wiki, using the user’s intent and confirmed routing preferences. If the destination is unclear, ask; don’t guess or create a wiki during routine ingestion.
- Remember confirmed routing preferences if agent memory is available, but don’t store document contents. This rule doesn’t require moving or deduplicating legacy documents.
- For sensitive records, confirm the destination when it isn’t explicit and follow applicable access controls.