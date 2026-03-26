[[Agile Specification Strategies]]

Agile documentation means writing just enough documentation to be useful — no more, no less.

The Agile Manifesto says "working software over comprehensive documentation." It does *not* say "no documentation." The key word is *comprehensive* — the bloated 200-page spec that nobody reads and nobody maintains.

Principles:
- **[[Document Continuously]]** — don't save documentation for the end. Write it as you go, as part of the development process.
- **[[Document Late]]** — only document things once they've stabilized. Documenting features that are still changing is waste.
- **[[Single Source Information]]** — every piece of information should live in exactly one place. Duplication leads to inconsistency.
- **[[Executable Specifications]]** — wherever possible, make your documentation executable (automated tests, BDD scenarios). If the documentation runs and passes, it's guaranteed to be current.

What to document:
- Architecture decisions and *why* they were made (ADRs — Architecture Decision Records)
- API contracts
- Onboarding guides for new team members
- Operational runbooks
- Anything that can't be understood by reading the code

What NOT to document:
- Anything the code already says clearly
- Detailed designs that will change next sprint
- Process for process's sake
- Documents that have no clear audience

The litmus test: if nobody would miss it, don't write it. If people would miss it, keep it short and keep it current.

Related: [[Test-Driven Development]], [[Agile Requirements]]
