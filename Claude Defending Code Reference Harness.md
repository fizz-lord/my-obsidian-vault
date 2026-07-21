---
type: research-note
status: open
severity: high
topic: llm-application-security
created: 2026-07-20
tags: [llm-application-security, vulnerability-hunting, open-source, frontier-models]
---

# Claude Defending Code Reference Harness

## What Happened
Anthropic released a reference harness for finding vulnerabilities, triaging them, and patching them with **Claude**. It implements a find grade patch pipeline inside Address Sanitizer instrumented Docker containers.

## Why It Matters
- Provides a concrete walkthrough for using frontier models in real vulnerability research pipelines.
- Shifts Claude from general purpose agent to repeatable security workflow primitive.
- Complements Datadog SAIST and Visa harness approaches.

## Source
- tldrsec #337
- https://github.com/anthropics/defending-code-reference-harness

## Related
- [[AI Security Index]]
- [[AI Red Teaming]]
- [[Autonomous LLM Vulnerability Hunting]]
