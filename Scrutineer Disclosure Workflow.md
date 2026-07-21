---
type: research-note
status: open
severity: high
topic: llm-application-security
created: 2026-07-20
tags: [llm-application-security, disclosure-workflow, agent-skills, open-source]
---

# Scrutineer Disclosure Workflow

## What Happened
**Alpha Omega Security's Scrutineer** runs agent skills in a container to scan repositories for security issues, triage findings, track maintainers, and manage disclosure workflows. It builds threat models, performs reachability analysis, and outputs structured reports.

## Why It Matters
- Goes beyond finding bugs to managing the full disclosure lifecycle, which is often the hardest part.
- Containerised agent skills provide reproducible review environments.
- Potential model for compliant AI assisted coordinators in vulnerability research programmes.

## Source
- tldrsec #337
- https://github.com/alpha-omega-security/scrutineer

## Related
- [[AI Security Index]]
- [[Autonomous LLM Vulnerability Hunting]]
- [[AI CEOs Converge on Regulation]]
