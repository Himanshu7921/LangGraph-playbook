# LangGraph vs LangChain (Working Notes)

Compare by re-implementing the same small task in both and noting differences.

## Criteria
- DX (setup, code clarity)
- Control Flow (branching, loops)
- Observability / Debugging
- Extensibility
- Performance (qualitative)

## Findings (TBD)
- ...

---

## Autonomicity and Control Flow

Levels of autonomicity observed in practice:
- L0: Rule-based if/else code → brittle, not scalable
- L1: Single LLM call (one agent) → shallow autonomy, hallucination risk
- L2: Chains → predefined paths, limited adaptability
- L3: Routing → dynamic branch selection per input
- L4: State machines (agentic graphs) → explicit nodes/edges/state, critic loops, termination

Where LangGraph helps
- Native graph abstraction: nodes, edges, shared state
- Conditional routing + loops: implement reviewer/critic cycles safely
- Observability: step-wise traces aligned to the graph

Where LangChain helps
- Quick composition of prompts/tools for linear chains
- Rich ecosystem of integrations

Takeaway
- Use LangChain for straightforward chains and integrations
- Use LangGraph when you need dynamic routing, feedback loops, and reliable autonomy
