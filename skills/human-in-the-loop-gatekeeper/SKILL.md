---
name: human-in-the-loop-gatekeeper
description: "Implements interruptible approval gates, operator escalations, and action confirmations."
---

# Human-in-the-Loop Gatekeeper

## Overview
The `human-in-the-loop-gatekeeper` skill injects deterministic pause states into autonomous agent workflows, requiring explicit human intervention before high-stakes actions are executed.

## Implementation Principles
1. **Interrupt Configuration:** Designate sensitive nodes (e.g., database writes, financial transactions, email dispatches) as interrupt boundaries.
2. **State Inspection:** Expose pending state payloads to the human operator for review or modification.
3. **Resume / Abort Logic:** Accept operator approval signals to resume execution or rejection directives to roll back changes.
