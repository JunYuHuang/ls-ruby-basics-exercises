# My Solution

It does not print.

The `a` variable defined in the top-most scope is referenced before it is defined. The `a` variable in the `each` call's block is local and not accessible outside of the block. Thus, the last line raises an error which stops the program.
