# Python List Methods Cheat Sheet

## 1. **Creating a List**
```python
my_list = [1, 2, 3, 4, 5]
print(my_list)
```

## 2. **Adding Elements**
```python
my_list.append(6)  # Adds element to the end
my_list.insert(2, 10)  # Inserts 10 at index 2
my_list.extend([7, 8, 9])  # Extends list with another list
print(my_list)
```

## 3. **Removing Elements**
```python
my_list.remove(10)  # Removes first occurrence of 10
popped = my_list.pop()  # Removes and returns last element
popped_index = my_list.pop(2)  # Removes and returns element at index 2
my_list.clear()  # Clears all elements
print(my_list)
```

## 4. **Finding Elements**
```python
my_list = [1, 2, 3, 4, 5, 3]
index = my_list.index(3)  # Returns first index of 3
count = my_list.count(3)  # Counts occurrences of 3
print(index, count)
```

## 5. **Sorting and Reversing**
```python
my_list.sort()  # Sorts in ascending order
my_list.sort(reverse=True)  # Sorts in descending order
my_list.reverse()  # Reverses the list
print(my_list)
```

## 6. **Copying a List**
```python
new_list = my_list.copy()  # Creates a copy of the list
print(new_list)
```

## 7. **List Comprehension**
```python
squared = [x**2 for x in my_list]  # Creates a new list with squared values
print(squared)
```

## 8. **Checking Membership**
```python
print(3 in my_list)  # Checks if 3 is in the list
print(10 not in my_list)  # Checks if 10 is not in the list
```

## 9. **Finding Maximum, Minimum, and Sum**
```python
print(max(my_list))  # Returns maximum value
print(min(my_list))  # Returns minimum value
print(sum(my_list))  # Returns sum of all elements
```

## 10. **Joining and Splitting Lists**
```python
words = ["Hello", "World"]
joined = " ".join(words)  # Joins list into a string
print(joined)
```

---
This cheat sheet covers essential Python list methods. 🚀
