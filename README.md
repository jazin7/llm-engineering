# Evaluating Agents

**Authors:** Leonard Gruber, Lukas Gruber, Yassine Ajoud

## Overview

This project investigates how to **evaluate AI agents**.

We build a small travel assistant agent with two tools (a weather lookup with fixed data and a calculator) and let two Qwen2.5 models answer 25 questions with known correct answers. We measure accuracy, tool use, robustness and efficiency.

## Goals

- Measure performance of agents.
- Compare agent behavior across different tasks.

## Milestones

- Milestone 1: Research
- Milestone 2: Create Framework
- Milestone 3: Compare Agents

## Files

- `main.ipynb`: all code, experiments and results
- `report.pdf` / `report.tex`: project report

## How to run

```
pip install transformers torch accelerate pandas matplotlib
```

Open `main.ipynb` and run all cells. The two models (about 4 GB) are downloaded from HuggingFace on the first run. On a laptop CPU the full run takes around 45 minutes.
