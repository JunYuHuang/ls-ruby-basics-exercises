# My Solution

The `map` method creates a new array that is the same size as the original array the method is called on. In the new array returned by `map`, each element is the return value of the block passed to `map`. The return value may also be `nil`. In this case, the `numbers.map` call with its passed block returns a new array that replaces all the odd (i.e. non-even) numbers in the original array with the `nil` value.

Fixed code:

```ruby
numbers = [5, 2, 9, 6, 3, 1, 8]

even_numbers = numbers.select do |n|
  n.even?
end

p even_numbers # expected output: [2, 6, 8]
```
