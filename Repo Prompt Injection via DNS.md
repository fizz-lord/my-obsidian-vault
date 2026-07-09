---
type: research-note
status: open
severity: high
topic: prompt-injection
created: 2026-07-03
tags: [prompt-injection, indirect-injection, agent-security, supply-chain]
---

# Repo Prompt Injection via DNS

## What It Is
0DIN demonstrates an **indirect prompt injection** attack against **Claude Code** that achieves full system compromise from a public GitHub repository containing **no malicious code**.

## Mechanism
- A benign `README` gives normal setup instructions
- A benign Python package throws a `RuntimeError` unless setup has run
- The setup script pipes a `dig` query to `bash`
- The **DNS TXT record** holds a base64 encoded reverse shell
- Claude Code automatically tries to fix the documented error, executing the payload

## Why It Matters
- The payload never appears in the repository itself
- Code review, static analysis, and agent file inspection all miss it
- The DNS record can be swapped anytime without new commits
- It exploits the model’s trained helpfulness rather than explicit malware

## Notes
- Relevant to trust boundary: public repo content should not be treated as safe instructions
- Permission mode matters: auto mode classifiers may behave differently from yolo mode execution

## Source
- tl;dr sec #336 / 0DIN

## Related
- [[AI Security Index]]
- [[Prompt Injection]]
- [[AI Red Teaming]]
- [[New MCP Spec Security Implications]]
