[[Agile Disciplines]]

Agile architecture is the practice of making architectural decisions just-in-time, evolving the system's structure as you learn more about what it needs to do.

The traditional approach: design the entire architecture upfront (Big Design Up Front / BDUF), create elaborate diagrams and documents, then implement. The problem: you're making your most critical structural decisions when you know the least about the system.

The agile approach: start with just enough architecture to get going ([[Architectural Envisioning]]), then let the architecture evolve as requirements and understanding deepen.

Principles:
- **Prove it with code** — architectural decisions should be validated through working software, not just diagrams. Build spikes and prototypes to test assumptions.
- **Delay decisions responsibly** — defer architectural choices until the "last responsible moment" — the point where not deciding costs more than deciding. This maximizes the information available for the decision.
- **Simple first** — start with the simplest architecture that could work. Complexity should be added in response to actual needs, not anticipated ones. YAGNI (You Aren't Gonna Need It) applies to architecture too.
- **Refactor as needed** — treat architecture as something that evolves. If a structural decision turns out to be wrong, change it. This requires good test coverage and disciplined refactoring practices.
- **Communicate through models** — use lightweight models (whiteboard sketches, simple diagrams) to communicate architectural intent. The model should be just detailed enough to be useful.

The tension: some decisions are genuinely hard to change later (database choice, programming language, deployment model). For these, invest more upfront thought. For everything else, defer and evolve.

Related: [[Agile Enterprise Architecture]], [[Agile Data Modeling]]
