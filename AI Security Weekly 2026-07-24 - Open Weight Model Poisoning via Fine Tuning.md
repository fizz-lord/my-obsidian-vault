---
title: Open-Weight Model Poisoning for Under $100 via Fine-Tuning
date: 2026-07-24
tags:
  - ai-security
  - model-poisoning
  - supply-chain
  - open-weight-models
  - backdoors
---

# Open Weight Model Poisoning for Under $100 via Fine Tuning

## What
Researcher Katie Paxton Fear demonstrated embedding persistent backdoors in open weight models using just 10 fine tuning examples (cost < $100). The poisoned model generated RCE vulnerable code on novel prompts, not just training examples. Larger models were easier to compromise. No reliable verification method exists for open weight model integrity.

## Why It Matters
Software supply chain attacks have moved to the model layer. Open weight models are opaque binaries with no equivalent of code review or SBOMs. Enterprises deploying fine tuned or third party open weight models have no practical way to detect embedded backdoors that activate conditionally.

## Source
https://x.com/v_shakthi/status/2078079582113341783

## Related
- [[AI Security Weekly 2026-07-24 - Sandworm_Mode Malware Living Off the AI Toolchain]]

#ai-security #model-poisoning #supply-chain #open-weight-models #backdoors
