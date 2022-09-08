# Checkout Action

This action performs a `git checkout`.

Checks out the expected branch regardless of who triggered the flow.

If the flow was triggered by a fork from someone other than Dependabot, exits.

This action is in a separate repo because:
- You can't call an action with a repo until after checkout
- The security checks cannot live within the same branch that is being tested

## Use

```
      - uses: MonarchEngineering/checkout-action@main
```
