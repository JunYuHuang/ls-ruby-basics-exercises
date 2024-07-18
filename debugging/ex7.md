# My Solution

The problem is that the `each` call's block overwrites the `balance` variable's value with the last iterated month's balance value. Instead, each iteration of the `each` call's block should cumulatively add the current month's balance value to `balance`.

Fix this by changing the `=` assignment operator in line 32 to the `+=` abbreviated assignment operator.
