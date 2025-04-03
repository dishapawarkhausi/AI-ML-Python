# Python Arrays

### What is an array in Python, and how is it different from a list?
An array is a collection of elements of the same data type, while a list can hold elements of different types. Arrays require the `array` module, while lists are built-in and more flexible.

### How do you create an array in Python using the array module?
Use the `array` module:
```python
import array
arr = array.array('i', [1, 2, 3, 4, 5])
print(arr)
```

### Write a Python program to create an array and print its elements.
```python
import array
arr = array.array('i', [10, 20, 30, 40, 50])
for element in arr:
    print(element)
```

### How do you access elements in an array using indexing?
Use indexing like lists:
```python
print(arr[0])  # First element
print(arr[-1]) # Last element
```

### Write a Python function to find the maximum and minimum elements in an array.
```python
def find_max_min(arr):
    return max(arr), min(arr)
arr = array.array('i', [3, 1, 9, 7, 2])
print(find_max_min(arr))
```

### How do you append an element to an array?
Use `append()`:
```python
arr.append(6)
```

### Write a Python program to insert an element at a specific index in an array.
```python
arr.insert(2, 99)  # Insert 99 at index 2
```

### How do you remove an element from an array?
Use `remove()` or `pop()`:
```python
arr.remove(3)  # Removes first occurrence of 3
arr.pop(1)     # Removes element at index 1
```

### Write a Python function to reverse an array.
```python
def reverse_array(arr):
    return arr[::-1]
arr = array.array('i', [1, 2, 3, 4])
print(reverse_array(arr))
```

### How do you find the length of an array?
Use `len()`:
```python
print(len(arr))
```

### Write a Python program to find the sum of all elements in an array.
```python
print(sum(arr))
```

### How do you sort an array in Python?
Use `sorted()`:
```python
arr = array.array('i', [4, 1, 3, 5])
sorted_arr = array.array('i', sorted(arr))
print(sorted_arr)
```

### Write a Python function to find the second largest element in an array.
```python
def second_largest(arr):
    unique_sorted = sorted(set(arr), reverse=True)
    return unique_sorted[1] if len(unique_sorted) > 1 else None
arr = array.array('i', [10, 20, 4, 45, 99])
print(second_largest(arr))
```

### How do you check if a specific value exists in an array?
Use `in`:
```python
if 10 in arr:
    print("Exists")
```

### Write a Python program to merge two arrays into one.
```python
arr1 = array.array('i', [1, 2, 3])
arr2 = array.array('i', [4, 5, 6])
merged = arr1 + arr2
print(merged)
```

### How do you convert a list into an array in Python?
```python
lst = [1, 2, 3]
arr = array.array('i', lst)
print(arr)
```

### Write a Python function to count occurrences of a specific element in an array.
```python
def count_occurrences(arr, val):
    return arr.count(val)
arr = array.array('i', [1, 2, 2, 3, 2, 4])
print(count_occurrences(arr, 2))
```

### How do you copy elements from one array to another?
```python
arr_copy = array.array('i', arr)
```

### Write a Python program to remove duplicate elements from an array.
```python
def remove_duplicates(arr):
    return array.array(arr.typecode, sorted(set(arr)))
arr = array.array('i', [1, 2, 2, 3, 4, 4])
print(remove_duplicates(arr))
```

### How do you iterate over an array using a loop?
```python
for element in arr:
    print(element)
