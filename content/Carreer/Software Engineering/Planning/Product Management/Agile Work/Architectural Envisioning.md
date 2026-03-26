[[Agile Session Types]] | [[Agile Architecture]]

Architectural envisioning is the initial, lightweight architecture work done at the beginning of a project. Just enough to establish the technical direction without over-designing.

The goal: identify the major architectural decisions that need to be made early and make them — while explicitly deferring everything that can wait until you know more.

What to figure out during architectural envisioning:
- **Technology stack** — programming language, frameworks, database, deployment platform. These are expensive to change later.
- **High-level structure** — monolith vs. microservices, major system components, key integration points.
- **Quality attributes** — how will you achieve the required performance, security, scalability, and reliability?
- **Constraints** — regulatory requirements, organizational standards, existing systems that must be integrated.
- **Risk areas** — where are the technical unknowns? What needs spike/prototype work to validate?

How to do it:
- Collaborative session with the technical team (and ideally a business representative)
- Use simple diagrams: component diagrams, deployment diagrams, sequence diagrams for critical flows
- Document decisions and their rationale — *why* you chose this approach, not just *what* you chose
- Plan architectural spikes for high-risk areas

How long: typically a few days. For a small project, maybe half a day. For a large enterprise system, maybe a week. Never months.

The principle: you're not designing the whole building. You're laying the foundation and framing the walls. The interior design happens iteratively as you build.

Related: [[Requirements Envisioning]], [[Iteration/Sprint Modeling]]
