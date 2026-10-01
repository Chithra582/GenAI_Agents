---
name: swarm-handoff-coordinator
description: "Configures multi-agent swarm handoffs, routine transfers, and shared state contexts."
---

# Swarm Handoff Coordinator

## Overview
The `swarm-handoff-coordinator` skill choreographs multi-agent collectives where specialized sub-agents hand off conversations and tasks dynamically via lightweight transfer routines.

## Coordination Mechanics
- **Transfer Functions:** Use explicit return functions (e.g., `transfer_to_triage_agent()`) as first-class tool calls.
- **Context Preservation:** Maintain shared memory variables across agent transitions to prevent redundant user questioning.
- **Recursion Ceiling:** Enforce a maximum handoff depth (default: 5 transfers) to eliminate endless ping-pong loops.
