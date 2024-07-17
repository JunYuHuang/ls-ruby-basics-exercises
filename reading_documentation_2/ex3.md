# My Solution

```ruby
s = 'abc def ghi,jkl mno pqr,stu vwx yz'

puts s.split.inspect
# Prints `"[\"abc\", \"def\", \"ghi,jkl\", \"mno\", \"pqr,stu\", \"vwx\", \"yz\"]"`

puts s.split(",").inspect
# Prints `"[\"abc def ghi\", \"jkl mno pqr\", \"stu vwx yz\"]"`

puts s.split(",", 2).inspect
# Prints `"[\"abc def ghi\", \"jkl mno pqr,stu vwx yz\"]"`

```
