# Python String Methods Cheat Sheet

## 1. **Basic String Operations**
```python
s = "Hello, World!"
print(len(s))  # Length of string
print(s[0])  # First character
print(s[-1])  # Last character
print(s[0:5])  # Substring (slicing)
```

## 2. **String Case Methods**
```python
print(s.lower())  # Convert to lowercase
print(s.upper())  # Convert to uppercase
print(s.capitalize())  # Capitalize first letter
print(s.title())  # Capitalize each word
print(s.swapcase())  # Swap case
```

## 3. **String Checking Methods**
```python
print(s.isalpha())  # Check if all characters are alphabetic
print(s.isdigit())  # Check if all characters are digits
print(s.isalnum())  # Check if all characters are alphanumeric
print(s.isspace())  # Check if string contains only whitespace
print(s.startswith("Hello"))  # Check if string starts with substring
print(s.endswith("World!"))  # Check if string ends with substring
```

## 4. **String Modification Methods**
```python
print(s.strip())  # Remove whitespace from both sides
print(s.lstrip())  # Remove whitespace from left side
print(s.rstrip())  # Remove whitespace from right side
print(s.replace("World", "Python"))  # Replace substring
```

## 5. **String Splitting and Joining**
```python
print(s.split(","))  # Split string into list
print("-".join(["Hello", "Python"]))  # Join list elements with separator
```

## 6. **String Searching Methods**
```python
print(s.find("World"))  # Find substring index (-1 if not found)
print(s.rfind("o"))  # Find last occurrence of substring
print(s.count("o"))  # Count occurrences of substring
```

## 7. **String Formatting**
```python
name = "Alice"
age = 25
print("My name is {} and I am {} years old.".format(name, age))  # Format using format()
print(f"My name is {name} and I am {age} years old.")  # Format using f-strings
```

## 8. **Encoding and Decoding**
```python
encoded = s.encode("utf-8")  # Encode string to bytes
print(encoded.decode("utf-8"))  # Decode bytes to string
```

## 9. **Checking Numeric Strings**
```python
num_str = "123"
print(num_str.isnumeric())  # True if all characters are numeric
print(num_str.isdecimal())  # True if all characters are decimal numbers
print(num_str.isdigit())  # True if all characters are digits
```

---
This cheat sheet covers essential Python string methods. 🚀
