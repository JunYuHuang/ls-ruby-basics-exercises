# My Solution

The problem is that `get_quote` returns `nil`. Any of the three `if` statements do not return a string; the string literals in the `if` statements do not return from the method.

Fix this problem by adding a `return` keyword in front of the string literal in each `if` statement.

Fixed code:

```ruby
def get_quote(person)
  if person == 'Yoda'
    return 'Do. Or do not. There is no try.'
  end

  if person == 'Confucius'
    return 'I hear and I forget. I see and I remember. I do and I understand.'
  end

  if person == 'Einstein'
    return 'Do not worry about your difficulties in Mathematics. I can assure you mine are still greater.'
  end
end

puts 'Confucius says:'
puts '"' + get_quote('Confucius') + '"'
```
