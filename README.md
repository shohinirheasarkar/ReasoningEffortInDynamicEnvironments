# Reasoning Effort in Dynamic Environments

> **Freshness-aware test-time compute for LLM agents operating in changing environments**

![Status](https://img.shields.io/badge/status-in%20development-f0ad4e)
![Course](https://img.shields.io/badge/UMD-CMSC%20473-E21833)
![Research](https://img.shields.io/badge/project-LLM%20agents-6f42c1)

## Overview

Language-model agents can often improve a decision by spending more time reasoning. In a dynamic environment, however, the world may change while the agent is thinking. A longer reasoning trace may therefore produce a more carefully considered answer based on information that is no longer current.

This project studies how an agent should balance:

- **decision quality** — whether additional reasoning improves the action;
- **reasoning cost** — the time and computation spent thinking; and
- **freshness** — whether the environment remains stable long enough for that reasoning to stay useful.

The goal is to develop a **freshness-aware test-time compute policy** that decides when an agent should continue reasoning, act immediately, or refresh its observation before acting.

## Research Question

> How should an LLM agent allocate reasoning effort when its environment can change during inference?

More specifically, can an agent estimate both task difficulty and environmental volatility, then use those estimates to choose a reasoning budget that improves performance without acting on stale information?

## Core Idea

Most test-time compute methods ask:

> *How difficult is this decision, and would more reasoning help?*

Our project adds a second question:

> *Will the information still be valid by the time the agent finishes reasoning?*

A freshness-aware agent may choose among three behaviors:

1. **Act now** when the decision is straightforward or the environment is changing quickly.
2. **Reason longer** when additional computation is valuable and the environment is sufficiently stable.
3. **Refresh and reconsider** when the original observation may have become stale.

## Planned Evaluation

We plan to compare freshness-aware reasoning against fixed-compute and difficulty-aware baselines in environments with controlled rates of change.

Key measurements may include:

- task success or decision quality;
- reasoning latency and compute usage;
- observation staleness at action time;
- regret caused by delayed action; and
- performance across different levels of environmental volatility.

Experimental details and benchmarks will be finalized as the project develops.

## Roadmap

- [ ] Finalize the formal problem definition
- [ ] Select or build dynamic evaluation environments
- [ ] Implement fixed-compute baselines
- [ ] Implement a difficulty-aware compute baseline
- [ ] Design the freshness or volatility estimator
- [ ] Implement the freshness-aware policy
- [ ] Run main experiments and ablations
- [ ] Analyze results
- [ ] Complete the report and presentation

Current work is tracked through the repository's **Issues** and **Projects** tabs.

## Team Workflow

1. Create or claim a GitHub Issue for a concrete task.
2. Assign the Issue and move it to **In Progress**.
3. Create a branch from `main`, such as `feature/12-volatility-estimator`.
4. Open a pull request when the work is ready for review.
5. Link the pull request with `Closes #12`.
6. Request a review from another team member.
7. Merge after review; the linked Issue will close automatically.

## Team

| Member | Role |
|---|---|
| Rhea Sarkar | Project member |
| Collaborator 1 | Project member |
| Collaborator 2 | Project member |

## Project Status

This project is currently in the research-design and early implementation stage. Methods, benchmarks, and results will be updated as experiments are completed.
