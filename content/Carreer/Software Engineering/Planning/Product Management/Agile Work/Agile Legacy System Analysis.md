[[Related Techniques in Agile]]

Legacy system analysis in an agile context is about understanding, integrating with, and incrementally modernizing existing systems — without rewriting everything from scratch.

Every organization has legacy systems. They're usually ugly, poorly documented, built on outdated technology, and absolutely critical to the business. The temptation is always "let's just rewrite it." The reality is that rewrites almost always take longer, cost more, and break more than anyone expected.

The agile approach to legacy systems:

**Understand first**
- Map what the system does (not how it does it). Focus on business capabilities, not code structure.
- Identify integration points — what depends on this system? What does it depend on?
- Talk to the people who use it. They know things the code doesn't tell you.

**Wrap, don't rewrite**
- Put an API or service layer around the legacy system. New features talk to the wrapper; the wrapper talks to the legacy system.
- This creates a seam — a point where you can gradually replace components without breaking everything.
- The Strangler Fig pattern: new functionality goes around the old system, gradually replacing it piece by piece, like a vine growing around a tree.

**Modernize incrementally**
- Replace the highest-risk or highest-value components first
- Each replacement should be small enough to ship safely
- Keep the old system running until the new component is proven in production
- Write tests for legacy behavior *before* changing it

**Accept what you can't change**
- Some legacy systems will outlive everyone reading this. If it works and the cost of replacing it exceeds the cost of maintaining it, leave it alone.
- Focus modernization effort where it creates actual business value.

The key insight: legacy systems aren't technical problems — they're business problems. The question isn't "how do we fix the code?" but "how do we reduce risk and increase capability?"
