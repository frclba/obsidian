# Agile Design

Agile design is the practice of doing just enough design, just in time, to support the current iteration of development. It's not "no design" -- that's a common misconception. It's the recognition that doing all your design upfront is wasteful because you don't yet know what you don't know. Requirements change, understanding deepens, and the best designs emerge through iterative refinement.

The relationship between agile design and [[Agile Architecture]] is important to understand. Architecture is the big-picture stuff -- the high-level structure, the major component boundaries, the technology choices that are hard to reverse. Design is more granular -- how individual classes interact, what patterns to use in a specific module, how to structure a particular feature. In agile, architecture gets a bit more upfront attention (because it's costly to change), while detailed design happens continuously throughout development.

The core principle is evolutionary design. You start simple, get something working, and then refactor as you learn more. This only works if you have strong engineering practices backing you up. [[Test-Driven Development]] is probably the most important one -- if you have a solid test suite, you can refactor with confidence. Without tests, refactoring is just gambling. TDD also drives better design naturally because code that's easy to test tends to be well-structured code.

[[how_to_software_engineer]] well in an agile context means being comfortable with ambiguity. You won't have a complete picture before you start building, and that's okay. The trick is to make decisions that are easy to reverse and defer decisions that are hard to reverse until you have more information. This is the "last responsible moment" principle -- don't decide before you need to, but don't procrastinate either.

[[Agile Modeling Session]]s are a great way to do collaborative design work. Get the team in front of a whiteboard, sketch out some ideas, debate the tradeoffs, and come to a shared understanding. The model doesn't need to be perfect or complete -- it just needs to be good enough to guide the next chunk of work. The whiteboard gets erased, the code captures the real design.

Some practical things that make agile design work: keep your classes small and focused, use interfaces to manage dependencies, apply design patterns when they fit naturally (not because you want to look clever), and refactor relentlessly. Technical debt is fine in small doses -- it's like taking on a loan to move faster. But if you never pay it down, the interest will crush you.

The biggest enemy of agile design is the fear of change. If the team is afraid to modify existing code, design stagnates. Building a culture where refactoring is expected, where the codebase is collectively owned, and where quality is everyone's responsibility -- that's what makes agile design actually work in practice.
