[[Agile Disciplines]] | [[Agile Architecture]]

Enterprise architecture in an agile context is about aligning the technical infrastructure of an entire organization while still allowing individual teams to move fast and make local decisions.

This is one of the hardest problems in scaling agile. When you have dozens or hundreds of teams, you need *some* level of coordination and shared standards — but too much central control kills the agility of individual teams.

The balance:
- **Guardrails, not gates** — instead of requiring approval for every architectural decision, establish principles and standards that teams must work within. Think highway lane markers, not tollbooths.
- **Shared platforms** — invest in common infrastructure (CI/CD pipelines, authentication, monitoring, data platforms) that teams consume as services. Teams shouldn't have to reinvent the wheel for cross-cutting concerns.
- **Architecture runway** — continuously invest in infrastructure work that enables future features. This work should stay ahead of the delivery teams, creating a "runway" they can build on.
- **Communities of practice** — instead of an ivory tower architecture team, create communities where architects from different teams share learnings, align on standards, and solve cross-team problems collaboratively.

The anti-patterns:
- Architecture team that says "no" to everything
- Standards so rigid that teams can't innovate
- No standards at all, resulting in chaos and integration nightmares
- Architecture disconnected from the people actually building things

The key insight: enterprise architecture should *enable* teams, not constrain them. If your architecture function is slowing teams down more than it's helping them, something is wrong.
