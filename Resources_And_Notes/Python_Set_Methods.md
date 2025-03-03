# Python Set Methods Cheat Sheet

## 1. **Creating a Set**
```python
set1 = {1, 2, 3, 4, 5}
set2 = set([3, 4, 5, 6, 7])  # Creating from a list
print(set1, set2)
```

## 2. **Adding Elements**
```python
set1.add(6)  # Add a single element
print(set1)
```

## 3. **Updating a Set**
```python
set1.update([7, 8, 9])  # Add multiple elements
print(set1)
```

## 4. **Removing Elements**
```python
set1.remove(3)  # Removes an element (raises error if not found)
set1.discard(10)  # Removes an element (no error if not found)
popped_element = set1.pop()  # Removes and returns a random element
set1.clear()  # Removes all elements
print(set1)
```

## 5. **Set Operations**
```python
set3 = {1, 2, 3, 4}
set4 = {3, 4, 5, 6}
print(set3.union(set4))  # Union of sets
print(set3.intersection(set4))  # Intersection of sets
print(set3.difference(set4))  # Difference (elements in set3 but not in set4)
print(set3.symmetric_difference(set4))  # Elements in either set, but not both
```

## 6. **Checking Subset & Superset**
```python
print(set3.issubset(set4))  # Check if set3 is a subset of set4
print(set3.issuperset({1, 2}))  # Check if set3 is a superset of another set
```

## 7. **Copying a Set**
```python
set_copy = set3.copy()  # Creates a copy of the set
print(set_copy)
```

## 8. **Frozen Sets (Immutable Sets)**
```python
frozen_set = frozenset([1, 2, 3, 4])  # Immutable set
print(frozen_set)
```

---
This cheat sheet covers essential Python set methods. 🚀
