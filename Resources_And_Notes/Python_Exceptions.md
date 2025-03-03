# Python Exceptions Cheat Sheet

## 1. **Handling Exceptions with try-except**
```python
try:
    x = 10 / 0  # This will raise a ZeroDivisionError
except ZeroDivisionError as e:
    print(f"Error: {e}")
```

## 2. **Catching Multiple Exceptions**
```python
try:
    value = int("abc")  # This will raise a ValueError
except (ValueError, TypeError) as e:
    print(f"Caught an error: {e}")
```

## 3. **Using finally (Always Executes)**
```python
try:
    file = open("test.txt", "r")
    content = file.read()
except FileNotFoundError as e:
    print("File not found!")
finally:
    print("Closing file...")
    file.close()
```

## 4. **Using else (Executes if No Exception)**
```python
try:
    num = int("5")  # No error here
except ValueError:
    print("Invalid number!")
else:
    print("Conversion successful!", num)
```

## 5. **Raising Exceptions Manually**
```python
def check_age(age):
    if age < 18:
        raise ValueError("Age must be 18 or older.")
    return "Valid Age"

try:
    print(check_age(15))
except ValueError as e:
    print(f"Exception: {e}")
```

## 6. **Custom Exceptions**
```python
class CustomError(Exception):
    pass

try:
    raise CustomError("This is a custom exception")
except CustomError as e:
    print(f"Caught CustomError: {e}")
```

## 7. **Common Built-in Exceptions**
| Exception | Description |
|-----------|-------------|
| `ZeroDivisionError` | Raised when dividing by zero |
| `ValueError` | Raised when an invalid value is used |
| `TypeError` | Raised when an operation is applied to an incorrect type |
| `IndexError` | Raised when an index is out of range |
| `KeyError` | Raised when a key is not found in a dictionary |
| `FileNotFoundError` | Raised when a file is not found |
| `AttributeError` | Raised when an invalid attribute is accessed |

---
This cheat sheet covers essential Python exception handling methods. 🚀
