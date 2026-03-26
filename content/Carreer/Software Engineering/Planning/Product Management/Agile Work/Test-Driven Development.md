[[Agile Specification Strategies]]

Test-Driven Development (TDD) is a simple discipline: write a failing test first, then write just enough code to make it pass, then refactor. Red, green, refactor. Repeat.

That's it. The entire practice fits in one sentence. But it changes how you write code fundamentally.

The cycle:
1. **Red** — write a test for behavior that doesn't exist yet. Run it. It fails. Good.
2. **Green** — write the minimum code to make the test pass. Don't be clever. Just make it work.
3. **Refactor** — now clean up. Remove duplication, improve naming, simplify structure. The tests ensure you don't break anything.

Why TDD works:
- **Forces design thinking** — before you write any code, you have to think about *what* it should do. This naturally leads to better interfaces and cleaner design.
- **Safety net** — your test suite grows with your codebase. Refactoring becomes safe because you'll know immediately if something breaks.
- **Documentation** — tests describe what the code does. New team members can read the tests to understand the system's behavior.
- **Confidence** — you can change code without fear. This is huge. Fear of breaking things is what causes codebases to rot.

Common objections:
- "It's slower" — it's slower *initially*. But you spend far less time debugging and reworking. Net time is usually less.
- "Not everything is testable" — true. UIs, integrations, and infrastructure are harder. TDD works best for business logic and domain code. Use other testing strategies for other layers.
- "Tests can have bugs too" — yes, but a test with a bug usually manifests as a false positive (test passes when it shouldn't), which gets caught when the real bug surfaces.

TDD isn't dogma. It's a tool. Use it where it helps. Skip it where it doesn't. But try it seriously before deciding it's not for you.

Related: [[Executable Specifications]], [[Agile Documentation]]
