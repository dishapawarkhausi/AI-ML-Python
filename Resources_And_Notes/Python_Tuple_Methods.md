# Python Tuple Methods Cheat Sheet

## 1. **Creating a Tuple**
```python
tuple1 = (1, 2, 3, 4, 5)
tuple2 = tuple([6, 7, 8])  # Creating from a list
print(tuple1, tuple2)
```

## 2. **Accessing Elements**
```python
print(tuple1[0])  # Access first element
print(tuple1[-1])  # Access last element
print(tuple1[1:4])  # Slicing a tuple
```

## 3. **Tuple Operations**
```python
tuple3 = tuple1 + tuple2  # Concatenation
print(tuple3)
print(tuple1 * 2)  # Repetition
```

## 4. **Checking Membership**
```python
print(3 in tuple1)  # Check if element exists
print(10 not in tuple1)
```

## 5. **Tuple Methods**
```python
tuple4 = (1, 2, 3, 2, 4, 2)
print(tuple4.count(2))  # Count occurrences of an element
print(tuple4.index(3))  # Find index of an element
```

## 6. **Unpacking Tuples**
```python
a, b, c = (10, 20, 30)  # Assigning values to variables
print(a, b, c)
```

## 7. **Iterating Over a Tuple**
```python
for item in tuple1:
    print(item)
```

## 8. **Finding Length, Max, and Min**
```python
print(len(tuple1))  # Length of tuple
print(max(tuple1))  # Maximum value
print(min(tuple1))  # Minimum value
```

## 9. **Converting Tuple to List and Vice Versa**
```python
list_from_tuple = list(tuple1)  # Convert tuple to list
tuple_from_list = tuple(list_from_tuple)  # Convert list to tuple
print(list_from_tuple, tuple_from_list)
```

---
This cheat sheet covers essential Python tuple methods. 🚀
