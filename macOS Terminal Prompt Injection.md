---
type: research-note
status: open
severity: high
topic: prompt-injection
created: 2026-07-20
tags: [prompt-injection, macos, terminal, indirect-injection]
---

# macOS Terminal Prompt Injection Trick

## What Happened
Security researcher Johann Rehberger disclosed a proof of concept that turns **indirect prompt injection into DNS exfiltration on macOS Terminal**. The injection flows from untrusted text through the terminal environment into the model context. Apple has already fixed the underlying behaviour.

## Why It Matters
- Broadens the attack surface for prompt injection beyond web UIs into local developer tooling.
- Terminal and shell bound agents are now in scope for indirect injection.
- Fix is OS-level, which means similar patterns likely exist in other terminal products.

## Source
- Daniel Miessler - Unsupervised Learning NO. 537
- Johann Rehberger post

## Related
- [[AI Security Index]]
- [[Prompt Injection]]
- [[AI Gateways as High Privilege Targets]]
