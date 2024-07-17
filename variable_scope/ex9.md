# My Solution

It prints `7`.

The `a` variable referenced to in the `each` call's block refers to the `a` parameter defined in the block's parameter list. This `a` parameter refers to the currently iterated element in `array` and thus does not affect the `a` variable defined outside the block.
