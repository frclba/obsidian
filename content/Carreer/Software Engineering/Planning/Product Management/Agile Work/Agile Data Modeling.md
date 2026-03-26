[[Agile Disciplines]]

Agile data modeling applies iterative, just-in-time principles to database design. Instead of designing the entire data model upfront, you evolve it alongside the application.

This is genuinely harder than agile application development because databases are *shared state*. Changing an application is relatively easy; changing a database schema that multiple systems depend on is risky.

Key practices:
- **Evolutionary design** — start with the simplest data model that supports your current features. Add tables, columns, and relationships as new features require them.
- **Database refactoring** — treat schema changes the same way you treat code refactoring. Rename columns, split tables, normalize or denormalize as needs become clear. The key is having tooling that makes this safe.
- **Migration scripts** — every schema change should be a versioned, reversible migration. Never modify the database by hand. Tools like Flyway, Liquibase, or framework-specific migrations make this manageable.
- **Test data management** — maintain test datasets that evolve with the schema. Automated tests should cover data integrity, not just application logic.
- **Collaborative modeling** — data models shouldn't be designed in isolation by a DBA. Developers, analysts, and domain experts should model together, ideally using whiteboard sessions.

The tension with agile data modeling is that some data decisions are truly hard to reverse — like choosing between relational and document databases, or fundamental entity relationship structures. For these foundational choices, invest more upfront thought. For everything else, evolve.

The goal: a data model that serves the application's current needs cleanly while remaining adaptable to future requirements.
