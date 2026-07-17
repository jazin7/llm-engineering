# Evaluating Agents

**Authors:** Leonard Gruber, Lukas Gruber, Yassine Ajoud

## Overview

LLM engineering course project. We build a small travel booking agent (search flights,
search hotels, book a trip under a budget) and run it with three local HuggingFace models.
Qwen2.5-3B, Falcon3-3B and SmolLM2-1.7B. The question is whether accuracy alone is enough to
evaluate an agent. Besides accuracy we measure robustness, efficiency, reliability, prompt
injection and recovery.

## Goals

- Measure performance of agents.
- Compare agent behavior across different tasks.

## Milestones

- Milestone 1: Research and task design
- Milestone 2: Create framework (marketplace, tools, agent loop, scoring)
- Milestone 3: Compare agents (Part I and Part II experiments)
- Milestone 4: Report and slides

## Files

- `travel_agent_evaluation.ipynb`: Part I. Agent, tasks and the main evaluation (accuracy, robustness, budget tiers, efficiency).
- `travel_agent_evaluation_part2.ipynb`: Part II. Prompt injection, reliability with sampling and recovery after a budget cut.
- `travel_agent_results.json` / `.csv`, `travel_agent_logs.json`: saved results and transcripts from Part I.
- `part2_*.json`: saved results from Part II.
- `exports/`, `exports2/`: charts, tables and findings from both parts.
- `report.pdf` / `report.tex`: project report.

## How to run

1. Put a HuggingFace token in a `.env` file next to the notebooks: `HF_TOKEN=hf_...`
2. Install the packages: `pip install transformers pandas numpy matplotlib tqdm python-dotenv`
   plus a CUDA build of PyTorch, e.g. `pip install torch --index-url https://download.pytorch.org/whl/cu128`.
3. Run the notebooks top to bottom.
