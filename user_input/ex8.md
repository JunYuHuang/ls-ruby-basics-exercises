# My Solution

```ruby
# `division.rb`

def valid_number?(number_string)
  number_string.to_i.to_s == number_string
end

loop do
  puts ">> Please enter the numerator:"
  numerator = gets.chomp
  if !valid_number?(numerator)
    puts ">> Invalid input. Only integers are allowed."
    next
  end

  puts ">> Please enter the denominator:"
  denominator = gets.chomp
  if denominator.to_i == 0
    puts ">> Invalid input. A denominator of 0 is not allowed."
    next
  end
  if !valid_number?(denominator)
    puts ">> Invalid input. Only integers are allowed."
    next
  end

  result = numerator.to_i / denominator.to_i
  puts "#{numerator} / #{denominator} is #{result}"
  break
end
```
