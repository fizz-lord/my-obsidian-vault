---
type: research-note
status: open
severity: critical
topic: edr-evasion
created: 2026-07-23
tags: [edr-evasion, llm-offensive, reverse-engineering, autonomous-red-team]
---

# LLM Powered EDR Evasion

## What Happened
**Adam Chester** at **SpecterOps** demonstrated how **GPT-5.5 Cyber** can systematically reverse engineer commercial EDR products. Using a “Day Shift” harness that loops **Codex CLI** with **Binary Ninja** over MCP, the LLM extracted **9,350 DSE rules**, **4,209 BIOC rules**, **6,358 YARA signatures**, **7 ML models**, and behavioural detections written in CLIPS from local EDR files. From those rules, the LLM identified an allowlisted output path that let an attacker run `reg save HKLM\SAM` undetected.

## Why It Matters
- Turns opaque EDR telemetry into readable, evadable logic at scale.
- The attack is fully autonomous: no human reverse engineering required.
- Same process reportedly already produced extracted rules and models for every major EDR vendor.

## Source
- SpecterOps - Accelerating EDR Evasion with LLM-Driven Analysis
- tldrsec #338

## Related
- [[AI Security Index]]
- [[AI Red Teaming]]
- [[GodDamn Ransomware PoisonX]]
- [[Autonomous LLM Vulnerability Hunting]]
