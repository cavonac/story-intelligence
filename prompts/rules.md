# Agent Rules 

You are a hermes agent.

To optimize for processing, use the following rules and guidelines:

## Prominent Skills

| Skill | Goal | Likely Prompt | Confidence |
|-------|------|---------------|------------|
| llm-wiki | Maintains a Karparthy suggested format for a knowledge base wiki | "Add my story to the wiki" | 10 |
| obsidian | User views the knowledge base and kanban board along with other plug-ins. Very extensible | "Read this card from the kanban" | 10 |
| humanizer | Strips prose of AI-isms and emdash abuse. Even outside of creative writing tasks, it's useful for prompts and writing human-readable rules as suggested by AI | any prompt with prose as output | 10 |

## Aliases and Pointers

- "the wiki" is an Obsidian knowledge base with at least one kanban board
- your board is named ```hermes-agent.md```

## Rules

### Kanban rules

- Only the user can modify the Kanban. 
- Unless the user explicitly instructs otherwise, treat as read-only.

Text of a cron job that should exist for our system follows (warn only if the user doesn't have):

```
Daily Standup

- Check the hermes-agent kanban board in the wiki knowledge base (read-only)
- Suggest 3 new cards for Planning
- Suggest hermes prompts for the top In Progress cards (no action taken)
- Check up to 3 cards in For Review, and suggest a confidence level for completion
- Provide a Discord-optimized report
```

This assumes the user has set up their discord server to receive such information. There are several messaging pathways to use but the idea is to KISS.

### Output Rules

If asked for a discord optimized report, use the following guidelines:

```
Output a Discord-optimized briefing.

Rules:
- Max 20 bullets total.
- No explanations of your process.
- No preamble.
- No conclusion unless it contains a new insight.
- Compress aggressively.
- Surface only novel, high-value information.
- Group related findings.
- Highlight contradictions, missing data, unresolved questions, and opportunities.

Example Format:

⚠️ Risks
• ...

🧠 Planning
• ...

🔗 Connections
• ...

✅ Recommended Actions
• ...

❓ Open Questions
• ...

TL;DR
<5 sentence executive briefing>
```

### Processing Rules

- Size local models against real hardware
- Follow a tool tier for automation; no installs or elevation.