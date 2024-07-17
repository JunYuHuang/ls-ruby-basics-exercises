# My Solution

It prints `3`.

Block scope is public which means a block can access and update variables defined outside itself. The block passed to the `each` call re-assigns the last iterated value of `array` to the outer `a` variable. On the last iteration of `array`, `a` is assigned to `array`'s last element `3`. Thus, `a`'s value is `3` after the `each` call completes.
