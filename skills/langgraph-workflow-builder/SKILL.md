---
name: langgraph-workflow-builder
description: "Constructs stateful graph cycles, memory checkpointers, and conditional branch routers."
---

# LangGraph Workflow Builder

## Overview
The `langgraph-workflow-builder` skill provisions cyclic state machines using LangGraph, incorporating persistent checkpointers, reducer functions, and dynamic conditional edge routing.

## Architectural Patterns
- **Cyclic Tool Loops:** Connect agent nodes with tool nodes, routing back into the agent until a stop condition is reached.
- **Durable Checkpointing:** Attach memory checkpointers (e.g., `MemorySaver`, PostgreSQL) to persist multi-turn conversational states.
- **Conditional Routers:** Define typed router functions that examine state values and select appropriate downstream nodes.
