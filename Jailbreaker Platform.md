---
type: research-note
status: open
severity: medium
topic: jailbreak
created: 2026-07-03
tags: [jailbreak, llm-security, testing, pyrit, red-team]
---

# Jailbreaker Platform

## What It Is
SpecterOps released **Jailbreaker**, an open source platform for repeatable LLM jailbreak testing.

## Features
- UI for configuring targets, running techniques, and tracking comparisons
- Technique registry includes direct and indirect prompt injection, roleplay, encoding obfuscation, system prompt extraction, and iterative attacks
- Supported iterative attacks: **PAIR**, **TAP**, **Crescendo**, **AutoDAN**, and **GPTFuzz**
- Reusable Target, Attacker, and Judge profiles
- Matrix experiments stored in **PostgreSQL** with SQL backed views

## Why It Matters
- Turns ad hoc jailbreak testing into an operator first workflow
- Docker Compose deployment lowers entry cost compared with composing Python primitives
- Useful comparison point against Microsoft's **PyRIT**

## Source
- tl;dr sec #336 / SpecterOps

## Related
- [[AI Security Index]]
- [[Jailbreak Techniques]]
- [[Emoji Jailbreaks]]
- [[AI Red Teaming]]
