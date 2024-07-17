# My Solution

```ruby
def time_of_day(is_daylight)
  if is_daylight
    puts "It's daytime!"
  else
    puts "It's nighttime!"
  end
end

daylight = [true, false].sample
time_of_day(daylight)
```
