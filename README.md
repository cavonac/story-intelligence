# Creative Writing "Story Intelligence" System

## Vision

This project exists to transform unstructured creative thought into discoverable story knowledge. 

I suffer from ADHD but not writer's block. As a result, I have a collection of disparate documents with different themes, settings, and characters that I want to synthesize into a coherent knowledge base wiki. Furthermore, I have a collection of these documents with which to process and a limited model agent at my disposal. I need a way to make an asynchronous pipeline for this work on my local data relatively safely. 

The primary input is not a finished manuscript.

The primary input is a large collection of fragmented creative material accumulated over time:

- Story ideas
- Scene fragments
- Character concepts
- Dialogue snippets
- Worldbuilding notes
- Research observations
- Theme explorations
- Alternative drafts
- Contradictory possibilities
- Incomplete narrative threads

These fragments may have been written months or years apart and often reference one another without explicit links. They are sometimes separated by a number dashes on a line, or by multiple blank lines (2-4). In this way, each snippet is written with the latest at the top and oldest at the bottom. I may have started and not finished other whole documents as well with overlapping concepts and themes. 

The goal of the system is to ingest this material, identify relationships, and construct an evolving knowledge graph that reveals patterns, connections, themes, and potential narratives that may not be obvious to the author. 

The system functions as a literary archaeology tool.

It excavates stories.

---

## Project Scope

This project is intentionally limited to the author's own work.

The system is not intended for:

- Public datasets
- Large external corpora
- Other authors' manuscripts
- Copyrighted fiction written by third parties
- Internet-scale ingestion

The purpose of the project is to help the author understand, organize, and develop a personal creative universe.

The graph should reflect the author's ideas rather than aggregate the ideas of others.

---

## Primary Workflow

```text
Creative Notes
     +
Scratch Documents
     +
Story Fragments
     +
Draft Chapters
     +
Research Notes
          │
          ▼

Document Ingestion

          ▼

Semantic Analysis

          ▼

Entity Extraction

          ▼

Relationship Discovery

          ▼

Knowledge Graph

          ▼

Obsidian Vault

          ▼

Story Discovery
```

---

## Core Concept

The system assumes that the author often does not know what story is being written yet.

Many fragments initially appear unrelated.

Over time, the graph should help identify:

- Recurring themes
- Repeated characters
- Similar concepts
- Emerging settings
- Narrative clusters
- Shared symbolism
- Potential plot structures

The graph is not merely documentation.

It is a mechanism for discovering structure hidden within creative chaos.

---

## Narrative Clustering

The system should automatically identify clusters of related ideas.

Example:

```text
Fragment A
    "Abandoned lighthouse"

Fragment B
    "Boy receives messages from the sea"

Fragment C
    "Flooded kingdom"

Fragment D
    "Moon controls tides"
```

These may have been written months apart.

The graph should discover that they belong to a common conceptual space and suggest a possible narrative cluster.

---

## Canon vs Possibility

Not every node in the graph represents canonical truth.

The system distinguishes between:

### Canon

Established facts.

### Candidate Knowledge

Potential ideas.

### Contradictions

Mutually exclusive concepts.

### Variants

Alternative story versions.

The graph should preserve uncertainty rather than prematurely resolving it.

---

## Local-First Philosophy

All story processing should occur locally whenever practical.

Goals:

- Preserve author privacy
- Protect unpublished intellectual property
- Maintain ownership of creative work
- Minimize external dependencies

Preferred components:

- Local LLMs
- Local vector databases
- Local graph databases
- Local embedding generation
- Local agent orchestration

The system should continue operating without cloud services whenever feasible.

---

## Human Voice Preservation

The system may use AI assistance during analysis and generation, but published prose must ultimately sound like the author.

Generated content should be treated as draft material.

Before incorporation into manuscripts, AI-produced text should pass through style-preservation or humanization workflows.

Potential tools include:

- Humanizer pipelines
- Local rewriting models
- Author-style refinement agents
- Manual editorial review

The objective is not to conceal AI use.

The objective is to ensure that the final prose reflects the author's voice rather than the default voice of a language model.

---

## Long-Term Goal

Build a continuously evolving creative intelligence system capable of:

- Reading years of creative material
- Extracting knowledge automatically
- Constructing a living story graph
- Identifying hidden relationships
- Preserving competing ideas
- Supporting worldbuilding
- Assisting manuscript development

The final product should function less like a writing assistant and more like a permanent literary research department for a single author.