# SWE_2021_41_2024_2_week6

## Week 4 Assignment
---
- [Link of repository](https://github.com/swoo7246/SWE_2021_41_2024_2_week_4)

### MY_CODE
```python
def isHappy(n):
  li = []
  while n != 1 and n not in li:
    li.append(n)
    a = 0
    for i in str(n):
      a += int(i)**2
    n = a
  return n == 1
```
- This function determines whether the input number n is a "happy number" by continuously calculating the sum of the squares of its digits until it either equals 1 or falls into a repetitive cycle.
---
