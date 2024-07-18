# My Solution

The `find_first_nonzero_among` method expects a single array parameter `numbers`. However, both examples do not pass such an argument; the first example passes a comma-separated list of integers, while the second examples passes a single integer.

The first example raises the `ArgumentError` error. The error message means the `find_first_nonzero_among` method received more arguments that are defined in the method's parameter list.

The second example raises the `NoMethodError` error. The error message means the `each` method does not exist on the `Integer` object argument passed to the `find_first_nonzero_among` call.

One way to fix both errors is to prefix the `numbers` array parameter in the `find_first_nonzero_among` method with a splat operator `*`. This way, the method can accept a comma-separated list of numbers of unknown length.
