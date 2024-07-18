# My Solution

The problem is that the local integer variable `product` is created with the value 0. This means no matter what number `product` is muiltiplied by, `product` will always be 0.

Fix the problem by initialising `product` with the value 1 in line 3.

Fixed code:

```ruby
def digit_product(str_num)
  digits = str_num.chars.map { |n| n.to_i }
  product = 1

  digits.each do |digit|
    product *= digit
  end

  product
end


p digit_product('12345')
# expected return value: 120
# actual return value: 0
```
