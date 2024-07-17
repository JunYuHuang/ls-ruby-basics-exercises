# My Solution

The code prints `7`.

The `my_value` method re-assigns the value of its parameter `a` by the `+=` operator. `+=` does not mutate the number (e.g. `a`) it operates on. Thus, when `my_value` is called with any number value, the passed number argument is not changed.

The `my_value` method has a parameter `a` shares the same name as the `a` variable in the outer scope. However, method definitions in Ruby are self-containing in terms of local variables; the outside `a` variable is not accessible inside the `my_value` method. Also, local variables (i.e. parameter) in a method are not accessible outside the method. Thus, the `a` referenced inside the `my_value` method must refer to the parameter defined inside `my_value`.
