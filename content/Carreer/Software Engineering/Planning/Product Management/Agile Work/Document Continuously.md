[[Agile Specification Strategies]] | [[Agile Documentation]]

Document continuously means treating documentation as an ongoing activity woven into the development process, not a phase at the end.

The traditional approach: build everything first, then write the documentation before release. The result: rushed, inaccurate docs written by people who've already mentally moved on to the next project.

The continuous approach:
- Write documentation *as* you build features
- Update docs when you change behavior
- Treat docs the same way you treat code — version controlled, reviewed, maintained
- Automate what you can (API docs from code, architectural diagrams from config)

What this looks like in practice:
- When a developer implements a feature, they also update the relevant documentation
- Architecture Decision Records (ADRs) are written when decisions are made, not months later from memory
- Runbooks are created when systems are deployed, not after the first outage
- README files evolve with the codebase

The key mindset: documentation is a *byproduct* of good development practices, not a separate deliverable. If your process naturally produces useful documentation, it stays current. If it requires a separate effort, it will always lag behind.

This pairs naturally with [[Executable Specifications]] — when your tests *are* your documentation, the continuous part happens automatically.

The balance: document what *needs* to be documented (architecture decisions, operational procedures, API contracts) and skip what doesn't (things the code already says clearly).

Related: [[Document Late]], [[Single Source Information]]
