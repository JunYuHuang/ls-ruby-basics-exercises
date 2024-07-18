# My Solution

The arrays `colors` and `things` are not the same length; `colors` has length 8 while `things` has length 7. Thus, when attempting to loop over both arrays using an int index that starts with 0 and ends with 7, index 7 is out of bounds for `things` whose last index is 6. In Ruby, out-of-bounds indexed elements in arrays have the value `nil` and `nil` cannot be implicitly converted to a string. Thus, Ruby raises an error and stops the program when the index `i` is 7.

The other problem is that the `if-statement` in the loop ensures that the index `i` will always be out of bounds because all arrays are 0-indexed in Ruby.

There are several ways to fix the problem but the principle is to ensure the index used to iterate through both arrays is never out-of-bounds for either array.

Fixed code:

```ruby
colors = ['red', 'yellow', 'purple', 'green', 'dark blue', 'turquoise', 'silver', 'black']
things = ['pen', 'mouse pad', 'coffee mug', 'sofa', 'surf board', 'training mat', 'notebook']

colors.shuffle!
things.shuffle!

i = 0
loop do
  break if i >= things.length

  if i == 0
    puts 'I have a ' + colors[i] + ' ' + things[i] + '.'
  else
    puts 'And a ' + colors[i] + ' ' + things[i] + '.'
  end

  i += 1
end
```
