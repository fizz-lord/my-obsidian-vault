---
type: research-note
status: open
severity: medium
topic: reinforcement-learning
created: 2026-07-03
tags: [reinforcement-learning, agent-training, github, coding-agents]
---

# Repo2RLEnv: GitHub as RL Environments

## What It Does
Turns existing GitHub repositories into reinforcement-learning environments using real development history.

## How It Works
- Issues become task definitions.
- Pull requests become example solutions.
- Commits and tests become behavior to learn from and verify.

## What Is Generated Per Task
- Starting repository state
- Goal to complete
- Automated evaluation logic
- Reward signal based on success

## Why It Matters
- Real repos provide continuously expanding RL task data.
- Benchmarks become dynamic rather than static and quickly saturated.
- The bottleneck shifts from model architecture to generating enough realistic environments.

## Security/AI Relevance
- Coding agents with weak or stale memory of code history train poorly on static benchmarks.
- Using live repo histories improves realism, attack-surface understanding, and evaluation.

## Related
- [[AI Security Index]]
- [[AI Red Teaming]]
