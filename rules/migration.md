# Migration of Creative Writing from Existing Wiki

You are a hermes agent, likely a local model. Users can start this task by asking you to perform phase 1, then 2, etc.

When migrating creative writing from an existing wiki, use the following guidelines

## Guidelines for Migration

Migrate my existing creative-writing content into a dedicated creative-writing wiki, following the installed `llm-wiki` skill and its Karpathy-inspired guidelines.

Work in distinct phases so destination setup can be done before or after migration:

### 1. Inspect and plan
- Read the `llm-wiki` skill instructions first; follow the installed version rather than assuming conventions.
- Identify the configured/current wiki location. Orient to it by reading its `SCHEMA.md`, `index.md`, and recent `log.md` entries when present.
- Inventory the current wiki and locate content that belongs to creative writing: fiction, characters, settings, plots, drafts, worldbuilding, and related notes.
- Summarize what you found, what should be migrated, and any ambiguous items. Keep unrelated wiki content out of scope.
- Do not modify or delete the source wiki during this phase.

### 2. Choose and prepare the destination — keep this phase independently executable
- Check whether a separate creative-writing wiki already exists. Consider the configured wiki location and other clearly identifiable wiki directories, but do not treat the general/current wiki as the creative-writing destination merely because it contains some writing notes.
- If a dedicated creative-writing wiki exists, use it and orient to its schema, index, and recent log before making changes.
- If none exists, propose a separate destination path and create a new wiki there using the skill’s initialization conventions. Do not overwrite an existing directory or change global wiki configuration without my approval.
- This phase may be completed before or after the content inventory. If it is deferred, finish the inventory and migration plan, then pause without writing migrated content until the destination is confirmed.

### 3. Migrate
- Preserve original files and content in the source wiki; treat it as read-only. Do not delete, rename, or overwrite source material.
- Follow the skill’s rules for raw sources, page structure, frontmatter, naming, cross-links, index updates, and append-only logging. Preserve provenance and distinguish original text from summaries or derived notes.
- Avoid inventing details, silently resolving contradictions, or flattening distinct drafts and versions into one. Flag ambiguity or conflicting versions for review.
- Reuse existing destination pages where appropriate and avoid duplicates. Keep pages scannable and split oversized pages according to the skill.
- If the work would touch 10 or more existing destination pages, stop and ask for approval before making those changes.

### 4. Validate and report
- Check that migrated files are present, links resolve, the destination index and log are updated, and the wiki passes the skill’s applicable lint/audit checks.
- Report the source and destination locations, what was migrated, what was left out or flagged, validation results, and any remaining decisions.
- Do not remove the source content after migration. Ask separately before any cleanup or archival action.
