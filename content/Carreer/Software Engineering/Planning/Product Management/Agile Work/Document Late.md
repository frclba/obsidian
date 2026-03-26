[[Agile Specification Strategies]] | [[Agile Documentation]]

Document late means waiting to create formal documentation until the information has stabilized. Don't document things that are still actively changing.

This isn't about procrastination — it's about efficiency. Writing detailed documentation for a feature design that will change three times before release is pure waste. You document it, it changes, you update the docs, it changes again, you update again... or more likely, you update once and then the docs silently drift out of sync.

The principle: document at the last responsible moment, when the information is stable enough to be worth capturing.

What this means in practice:
- **Don't** write detailed design docs during early iteration when designs are fluid
- **Do** write them once the design has stabilized through implementation and feedback
- **Don't** document APIs before they're built and tested
- **Do** document APIs once they're proven and stable
- **Don't** write user guides for features that might be redesigned
- **Do** write user guides once the UX is settled

This pairs with [[Document Continuously]] — you document continuously *once things are stable enough to document*. Before that, use lightweight artifacts: whiteboard sketches, sticky notes, conversation.

The risk of documenting early isn't just wasted effort — it's *wrong documentation*. Outdated docs are worse than no docs because people trust them and make bad decisions.

Related: [[Document Continuously]], [[Single Source Information]], [[Agile Documentation]]
