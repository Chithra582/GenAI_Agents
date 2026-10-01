---
name: trace-eval-benchmark-suite
description: "Benchmarks agent traces for faithfulness, answer relevance, latency, and token cost."
---

# Trace Eval & Benchmark Suite

## Overview
The `trace-eval-benchmark-suite` skill provides quantitative evaluation methodologies to measure agent quality across production execution trajectories.

## Evaluation Metrics
1. **Faithfulness:** Degree to which generated assertions are supported by retrieved context.
2. **Answer Relevance:** Semantic alignment between the user's initial question and the agent's final response.
3. **Step Efficiency:** Number of tool calls and intermediate turns required to reach task resolution.
4. **Cost & Latency:** Total token consumption and execution latency across distributed tool invocations.
