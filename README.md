# Story Intelligence

Story Intelligence turns a collection of personal writing fragments into an evolving knowledge base. It uses [LLM-Wiki](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f) as a "pattern for building personal knowledge bases using LLMs" (Karpathy, 2026) by organizing my story ideas which then helps surface connections, continuity issues, themes, and possible story directions.

## Why

I suffer from ADHD, but not writer's block because it provides a lot of focus and creativity. Unfortunately, I have an unorganized collection of documents with different themes, settings, and characters that I want to synthesize into a coherent knowledge base wiki. Furthermore, I have a limited model agent at my disposal. I need a way to perform asynchronous work on my local data with relative safety.

The goal is to make it easier to explore my own work in a knowledge base and discover patterns I might otherwise miss.

I also have a background in software engineering, so this project should follow modern engineering best practices wherever they make the system more reliable, secure, and maintainable. I plan to keep the design practical: avoid unnecessary complexity, but not sacrifice sound architecture for a quick prototype.

Examples include:

- Use clear module boundaries and well-defined interfaces between stages.
- Validate configuration and input data, and handle failures and retries explicitly.
- Add automated tests for core behavior, especially ingestion, parsing, and graph updates.
- Protect local data with sensible permissions, safe file handling, and documented backup and recovery procedures.
- Track dependencies and document setup, operational assumptions, and significant design decisions.
- Use structured logging and basic monitoring so scheduled runs are easy to inspect and troubleshoot.

## What it does

The pipeline can ingest creative material asynchronously and run on a schedule. It’s designed to:

- Extract characters, settings, concepts, and relationships
- Group related fragments into possible narrative clusters
- Surface recurring themes, symbols, and story threads
- Preserve contradictions, alternate versions, and uncertainty
- Export an evolving knowledge base to an Obsidian vault

Inputs may include story ideas, scene fragments, dialogue, world-building, research notes, draft chapters, and unfinished narrative threads. In some documents, fragments are separated by dashes or blank lines, with newer notes near the top and older ones below.

## Pre-requisites

- I use [Obsidian](https://obsidian.md/) to view the KB and the knowledge graph
- To schedule jobs for ingestion and massaging the data I use a [Hermes Agent](https://hermes-agent.nousresearch.com/) with a local model
- In addition to the KB, I've added a kanban board for obvious reasons. The version I use is the [community plug-in](https://community.obsidian.md/plugins/obsidian-kanban) simply called 'Kanban'.

## How it works

```text
Creative notes and drafts
          ↓
Document ingestion
          ↓
Semantic analysis and entity extraction
          ↓
Relationship discovery
          ↓
Knowledge graph
          ↓
Obsidian vault
          ↓
Story discovery
```

For example, notes about an abandoned lighthouse, messages from the sea, a flooded kingdom, and the tides might be connected as a potential story cluster, even if they were written months apart.

A lot of the heavy lifting is done by the agent, so results may vary, even on multiple runs using the same data. It is up the user to modify their implementation locally as needed, making this system portable for anyone running agentic software now or in the future.

## Canon and possibilities

The graph should distinguish between:

- **Canon:** established facts
- **Candidate knowledge:** ideas that may become part of a story
- **Contradictions:** ideas that cannot all be true at once
- **Variants:** alternate versions of a character, setting, or story

The system should preserve these distinctions rather than resolve them automatically.

## Local-first and project scope

This project is intended for my own creative work, not public datasets, large external corpora, or other authors’ manuscripts. Processing should happen locally whenever practical, using local models, embeddings, databases, and orchestration tools. The system should remain useful without cloud services where feasible.

## Using AI-generated material

AI can help analyze the notes and suggest connections or draft material. Suggestions remain drafts for review; published prose should reflect my voice and go through my own editorial process. The goal is to support the writing, not conceal AI involvement.

## Setup

1. Review [`agents/setup.md`](./agents/setup.md) for installation guidance.
2. Update [`config/setup.yaml`](./config/setup.yaml) for your system and preferences before setup.
3. Start with [`agents/agents.md`](./agents/agents.md) for the agent workflow.


## Long-term goal

Build a personal literary research system that can organize years of creative work, preserve competing ideas, reveal hidden connections, and support world-building and manuscript development.