# Python Dictionary Methods Cheat Sheet

## 1. **Creating a Dictionary**
```python
my_dict = {"name": "Alice", "age": 25, "city": "New York"}
print(my_dict)
```

## 2. **Accessing Values**
```python
print(my_dict["name"])  # Access value using key
print(my_dict.get("age"))  # Access value safely (returns None if key not found)
```

## 3. **Adding & Updating Values**
```python
my_dict["job"] = "Engineer"  # Adding a new key-value pair
my_dict["age"] = 26  # Updating an existing key
print(my_dict)
```

## 4. **Removing Elements**
```python
del my_dict["city"]  # Remove key-value pair by key
removed_value = my_dict.pop("age")  # Remove key and return its value
last_item = my_dict.popitem()  # Remove and return last inserted item
my_dict.clear()  # Remove all items
print(my_dict)
```

## 5. **Checking Keys & Values**
```python
print("name" in my_dict)  # Check if key exists
print(my_dict.keys())  # Get all keys
print(my_dict.values())  # Get all values
print(my_dict.items())  # Get all key-value pairs
```

## 6. **Copying a Dictionary**
```python
new_dict = my_dict.copy()  # Creates a copy of the dictionary
print(new_dict)
```

## 7. **Merging Dictionaries**
```python
other_dict = {"country": "USA", "hobby": "Reading"}
my_dict.update(other_dict)  # Merge two dictionaries
print(my_dict)
```

## 8. **Using Dictionary Comprehension**
```python
squared_numbers = {x: x**2 for x in range(5)}
print(squared_numbers)
```

## 9. **Setting Default Values**
```python
value = my_dict.setdefault("gender", "Female")  # Returns value if key exists, else sets default
print(my_dict)
```

---
This cheat sheet covers essential Python dictionary methods. 🚀
