# My Solution

```ruby
# `lsprint2.rb`

loop do
  puts '>> How many output lines do you want? Enter a number >= 3: (Q to quit)'
  input = gets.chomp

  break if input.downcase == 'q'

  line_count = input.to_i
  if line_count < 3
    puts ">> That's not enough lines."
    next
  end

  while line_count > 0
    puts 'Launch School is the best!'
    line_count -= 1
  end
end
```
