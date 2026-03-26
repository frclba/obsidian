[[Agile Specification Strategies]]

Executable specifications are requirements documents that can be run as automated tests. The spec *is* the test. When it passes, the system meets the requirement. When it fails, it doesn't.

This is one of those ideas that sounds obvious in hindsight but changes everything in practice. Traditional specs sit in a document, slowly drifting out of sync with the actual system. Executable specs can't drift — they're verified every time the test suite runs.

The main approach: **Behavior-Driven Development (BDD)**

BDD uses a Given-When-Then format that's readable by both business people and developers:
- **Given** some initial context (the world is in this state)
- **When** an event occurs (the user does something)
- **Then** ensure some outcome (this should be true)

Example:
> Given a user has items in their cart
> When they apply a valid discount code
> Then the total should reflect the discount

This scenario is simultaneously: a requirement, a test case, and living documentation.

Tools: Cucumber, SpecFlow, Behave, and similar frameworks let you write these scenarios in plain language and connect them to automated test code.

Benefits:
- Requirements and tests are the same thing — no translation errors
- Always up-to-date documentation
- Business people can read and validate the specs
- Forces clarity — vague requirements become obvious when you try to make them executable

The catch: writing good executable specs requires skill. Bad BDD scenarios end up being brittle, verbose, and harder to maintain than the tests they replace. Focus on behavior, not implementation details.

Related: [[Test-Driven Development]], [[Agile Documentation]], [[Document Continuously]]
