---
type: research-note
status: open
severity: medium
topic: agent-memory
created: 2026-07-03
tags: [agent-memory, context-management, ai-agents]
---
# Long Term Memory for AI Agents

## Problem
Agents forget user preferences, corrections, and prior context across sessions; vector databases alone do not fix this.

## Why Vector DBs Fall Short
- They store embeddings, not truth.
- Outdated facts and corrections remain side by side.
- Multi-session, multi-entity memory requires structured reasoning over time.

## Key Concepts
- Context window: what the model sees now.
- Long-term memory: what persists after the session ends and must stay accurate weeks later.
- Pre-clean context matters: system prompt, history, tool descriptions, and retrieved docs often consume a large portion of context.

## Memory Scopes
- User: individual preferences, history, corrections
- Customer/org: shared context
- Client/product: relationship-specific context
- World: general knowledge

## Defensive/Practical Notes
- Manage what is current versus outdated before retrieval.
- Resolve entities across sessions instead of duplicating people/facts.
- Keep accuracy, relevance, and timeliness explicit in agent context handling.

## Related
- [[AI Security Index]]
- [[AI Red Teaming]]
