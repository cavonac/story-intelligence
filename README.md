# Story Intelligence

Story Intelligence turns a collection of personal writing fragments into an evolving knowledge base. It uses LLM-Wiki to organize ideas into a knowledge graph, then helps surface connections, continuity issues, themes, and possible story directions.

## Why

I suffer from ADHD but not writer's block. As a result, I have a collection of disparate documents with different themes, settings, and characters that I want to synthesize into a coherent knowledge base wiki. Furthermore, I have a limited model agent at my disposal. I need a way to make an asynchronous pipeline for this work on my local data with relative safety.

The goal is to make it easier to explore my own work in a knowledge base and discover patterns I might otherwise miss.

## What it does

The pipeline can ingest creative material asynchronously and run on a schedule. It’s designed to:

- Extract characters, settings, concepts, and relationships
- Group related fragments into possible narrative clusters
- Surface recurring themes, symbols, and story threads
- Preserve contradictions, alternate versions, and uncertainty
- Export an evolving knowledge base to an Obsidian vault

Inputs may include story ideas, scene fragments, dialogue, world-building, research notes, draft chapters, and unfinished narrative threads. In some documents, fragments are separated by dashes or blank lines, with newer notes near the top and older ones below.

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

For example, notes about an abandoned lighthouse, messages from the sea, a flooded kingdom, and the tides might be connected as a potential story cluster—even if they were written months apart.

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