---
type: research-note
status: open
severity: high
topic: prompt-injection
created: 2026-07-03
tags: [prompt-injection, red-teaming, attack-surface]
---

# Prompt Injection as Role Confusion

## Key Idea
Prompt injection succeeds because models infer roles from writing style, not from structural tags.

## Attack Mechanisms
- CoT Forgery: fake reasoning injected in user prompts that mimics model thinking style, raising attack success from near-zero to ~60% across frontier models.
- Role spoofing via style: prepending `User:` to malicious tool output increases injection success.
- Subconscious steering: non-malicious text style shifts model behavior without direct injection.

## Defensive Notes
- Do not rely on XML/JSON-style structural tags alone for trust boundaries.
- Treat reasoning-style text with caution even when it claims to be user input.
- Probe per-role metrics such as CoTness and Userness with linear probes when auditing models.

## References
- Charles Ye, Jasmine Cui, Dylan Hadfield-Menell, ICML 2026
- Code: role-confusion/prompt-injection-as-role-confusion

## Related
- [[Prompt Injection]]
- [[AI Red Teaming]]
- [[Jailbreak Techniques]]
