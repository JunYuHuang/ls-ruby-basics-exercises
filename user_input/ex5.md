# My Solution

```ruby
# `lsprint.rb`

loop do
  puts ">> How many output lines do you want? Enter a number >= 3:"
  count = gets.to_i

  if count < 3
    puts ">> That's not enough lines."
    next
  end

  count.times { puts "Launch School is the best!" }
  break
end
```
