# Rulealize.RuleSet.PackingList

What to take, and what is in the bag already: items added as they come to mind and ticked as they are packed. A [Rulealize](https://github.com/reny-develop/Rulealize) rule set.

| | |
| --- | --- |
| Rule set id | `Rulealize.RuleSet.PackingList` |
| Package | [`Rulealize.RuleSet.PackingList`](https://www.nuget.org/packages/Rulealize.RuleSet.PackingList) |
| Inputs | `add`, `pack`, `unpack`, `remove` |
| Holds | nothing |
| Draws on | TypeSchema, State, Sequence, Comparison, Logic, Binding, Branch, Definition |

Nothing ends it: a list for the next trip is the same list with everything unpacked.

| Projection | Holds |
| --- | --- |
| `left` | What is listed and not yet packed |
| `packed` | What is in the bag |
| `list` | Every item, `{ "item", "state" }`, `state` being `packed` or `left` (added in 1.1) |
| `counts` | How many are `left`, `packed`, and listed in `all` (`all` added in 1.1) |

## Opening it

[Rulpane](https://github.com/reny-develop/Rulpane) opens it from the
[Rulealize Registry](https://github.com/reny-develop/Rulealize.Registry) by its identifier and
version: `#r=Rulealize.RuleSet.PackingList@1.1.0`.

## License

[Apache-2.0](LICENSE).
