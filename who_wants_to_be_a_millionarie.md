## Any interest?

Write a function
```python
get_balance(initial_balance, num_days, annual_interest_rate)
```

Gets the balance if we started with `initial_balance` after `num_days`, if there is an interest rate of `annual_interest_rate`, compounded daily

Examples:
```python
>>> # put $1k in a 0% account for a year
>>> get_balance(1000.00, 365, 0.0) 
1000.00

>>> # put $1k in a 4% APR account for a year. Note that because of compound interest
>>> # the number is bigger than $1040 ($40 is 4% of $1k) 
>>> get_balance(1000.00, 365, 0.04)  # put $1k in a 4% APR accoun
$1040.8085
```

### Skills

- Practice writing functions
- Docstring best practices
- Using keyword arguments for clarity
- Calculation of compound interest
- Use of for loops and/or exponents

## How long to be a millionaire?

Write a function given an interest rate and an initial balance, how many days it would take for the balance reaching one million dollars. That is, what is the _smallest_ number of days we would have to wait before we reach one million dollars or more?


