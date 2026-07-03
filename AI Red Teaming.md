---
type: research-note
status: open
severity: high
topic: red-teaming
created: 2026-07-03
tags: [red-teaming, ai-security, attack-surface]
---

# AI Red Teaming

**Tags:** `#red-teaming #ai-security`

## Overview
Red teaming for AI systems involves structured adversarial testing.

## Related Topics
- [[Prompt Injection]]
- [[Jailbreak Techniques]]
- [[Model Extraction]]

## Methodology Checklist
- Define target model and scope.
- Identify attack surface.
- Run prompt injection tests.
- Document jailbreak successes and failures.
- Attempt extraction attacks.
- Write report with mitigations.

## Workflow: Structured Red Team Assessment
Input: target model details.
Output: vulnerability report.

Steps:
1. Load model card and API documentation.
2. Map expected behavior.
3. Probe with adversarial prompts.
4. Attempt data or weight extraction.
5. Write report with mitigations.

## Backlinks
- [[AI Security Index]]
