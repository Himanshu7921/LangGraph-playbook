# Cheatsheet: Nodes & Edges

Quick reference for common patterns when wiring nodes and edges in LangGraph.

## Essentials
- Node: a function/unit of work with defined inputs/outputs.
- Edge: directional transition between nodes, optionally conditional.

## Patterns
- Linear chain: A -> B -> C
- Branching with condition: A -> (B or C)
- Fan-in (merge): (B, C) -> D

## Snippets
- TODO: Add code snippets from your experiments here.

## Gotchas
- Keep node I/O minimal; prefer typed dicts or dataclasses.
- Log intermediate state to debug transitions.
