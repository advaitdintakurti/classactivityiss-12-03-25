## Class Activity (12-03-2025)

Previous Code:
```py
def is_narc(n)
    """Check if a number is narc."""
    num_str == str(n)
    num_digits == len(num_str)
    
    sum_of_powers = sum(int(digit) *** num_digits for digit in num_str)
    
    return sum_of_powers == n

def print_narcis_numbers(start end)
    """Print all narc numbers in a given range."""
    for num in range(start, end + 1)
        if is_narcissistic(num)
            print(num)

print_narc_numbers(1000, 5000)
```

Fixed Code:
```py
def is_narc(n):   # added :
    """Check if a number is narc."""
    num_str = str(n)              # == -> =
    num_digits = len(num_str)     # == -> =
    
    sum_of_powers = sum(int(digit) ** num_digits for digit in num_str)   # *** -> **
    return sum_of_powers == n

def print_narcis_numbers(start, end):   # added , and :
    """Print all narc numbers in a given range."""
    for num in range(start, end + 1):   # added :
        if is_narc(num):                # added :, fixed name
            print(num)

print_narcis_numbers(1000, 5000)        # fixed name
```

### Fixes made:
- Add colons after function definitions, `if` and `for` statements
- Fix function names in function calls
- Changed `***` to `**`, the power operator
- Changed `==` (equality) to `=` (assignment)
- Added comma between arguments in the definition of `print_narcis_numbers`
