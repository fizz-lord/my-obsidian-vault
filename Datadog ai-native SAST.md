---
type: research-note
status: open
severity: high
topic: llm-application-security
created: 2026-07-20
tags: [llm-application-security, sast, open-source, ai-native]
---

# Datadog ai-native SAST

## What Happened
**Datadog** released a preview-stage AI-native SAST tool that uses large models to find vulnerabilities in Java, Python, and Go code, then emits SARIF reports. Detection and validation stages use Anthropic, OpenAI, and Gemini models separately.

## Why It Matters
- Confirms mainstream security vendors are productising LLM-based code analysis.
- Detection prompts are fetched from Datadog's hosted API, introducing a new supply-chain trust consideration.
- Output standardisation via SARIF eases integration into existing CI pipelines.

## Source
- tldrsec #337
- https://github.com/DataDog/datadog-saist

## Related
- [[AI Security Index]]
- [[Claude Defending Code Reference Harness]]
- [[Visa Vulnerability Agentic Harness]]
