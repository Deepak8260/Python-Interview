# Numbers

###### ` Question 1: Convert String to Number`
Converting a string representation of a number to an integer or a float is straightforward in Python.

##### `Approach : Using int() or float() Functions`
- int(): Converts a string containing an integer to an integer.
- float(): Converts a string containing a decimal number to a floating-point number.

`Example`
```python
def convert_string_to_number(s):
    //Your Code Here

# Example usage
print(convert_string_to_number("42"))    # Output: 42 (int)
print(convert_string_to_number("42.3"))  # Output: 42.3 (float)
```

`References:`
- [Python int() documentation](https://docs.python.org/3/library/functions.html#int)
- [Python float() documentation](https://docs.python.org/3/library/functions.html#float)

<details>
  <summary>Solution</summary>

### Lets Explore the Solution:

```python
def convert_string_to_number(s):
    try:
        # Try converting to an integer first
        result = int(s)
    except ValueError:
        # If conversion to integer fails, try converting to a float
        result = float(s)
    return result

# Example usage
print(convert_string_to_number("42"))    # Output: 42 (int)
print(convert_string_to_number("42.3"))  # Output: 42.3 (float)
```

**Explanation:**
1. Use a try block to attempt converting the string to an integer using int().
2. If the string contains a decimal point, int() will raise a ValueError. The except block catches this error and converts the string to a float using float().

  
</details>











