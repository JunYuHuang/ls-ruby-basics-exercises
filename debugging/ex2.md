# My Solution

The original code's `predict_weather` method results in the same output every time because its local array variable holds two strings. In Ruby, all strings are evaluated as truthy. No matter which element is randomly picked and stored in the `sunshine` variable, `sunshine` would be evaluated as truthy. Thus, the `else` clause of the `if-else` expression never executes. The problem can be fixed by replacing two strings in that array with the two boolean values `true` and `false`.

Fixed code:

```ruby
def predict_weather
  sunshine = [true, false].sample

  if sunshine
    puts "Today's weather will be sunny!"
  else
    puts "Today's weather will be cloudy!"
  end
end
```
