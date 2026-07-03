---
type: research-note
status: open
severity: medium
topic: mcp-security
created: 2026-07-03
tags: [mcp-security, agent-protocol, attack-surface]
---

# New MCP Spec Security Implications

## Spec Status
Target release: 2026-07-28

## Key Changes
- Stateless architecture.
- OAuth 2.1 with PKCE mandated.
- Removes protocol-level session hijacking, unsolicited server prompts, and weak authentication.

## New Attack Surfaces
- Cross-agent workflow hijacking via predictable tracking IDs or unverified state.
- Client-controlled metadata manipulation through unsigned `_meta` objects.
- Desync attacks via new MCP-specific headers.
- Stored XSS through interactive MCP Apps.
- Denial-of-service via long-running async tasks.

## Practical Takeaway
Security shifts from protocol hardening to correct implementation of trust boundaries, state management, and execution models in MCP apps.

## Related
- [[AI Security Index]]
- [[AI Red Teaming]]
