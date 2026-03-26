[[Agile Specification Strategies]] | [[Agile Documentation]]

Single Source Information means every piece of information lives in exactly one authoritative place. If you need to update something, you update it in one place and it's done. No hunting, no syncing, no conflicting versions.

The problem it solves: information duplication. When the same fact exists in a requirements doc, a wiki page, a design document, and a slide deck, they will inevitably diverge. Then people make decisions based on different versions of the truth and things break.

How to apply it:
- **Code is the single source for behavior** — if someone asks "what does this system do?", the code is the authority, not a design document.
- **Tests are the single source for expected behavior** — [[Executable Specifications]] make this automatic.
- **One wiki, not three** — pick one documentation platform and commit to it. Don't spread documentation across Confluence, Google Docs, Notion, and a shared drive.
- **Configuration lives in config** — not in documentation, not in people's heads, not in email threads. In the actual configuration files, version controlled.
- **Architecture decisions in ADRs** — one file per decision, with context, options considered, and rationale.

The DRY principle (Don't Repeat Yourself) from software development applies to documentation too. If information exists in two places, one of them will be wrong.

Practical tip: when you notice duplicate information, don't just update both copies. Delete one and replace it with a link to the other. Reduce the number of sources, one at a time.

Related: [[Document Continuously]], [[Document Late]], [[Agile Documentation]]
