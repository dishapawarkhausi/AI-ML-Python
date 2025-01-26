# ⚡ NumPy Universal Functions (ufunc) Guide

NumPy Universal Functions (ufuncs) are optimized functions that perform element-wise operations on arrays. They are fast, efficient, and support broadcasting, type casting, and custom operations.

## 📌 Importing NumPy
```python
import numpy as np
```

## 🔢 Basic Arithmetic ufuncs
```python
a = np.array([1, 2, 3, 4])
b = np.array([5, 6, 7, 8])

print(np.add(a, b))  # Element-wise addition
print(np.subtract(a, b))  # Element-wise subtraction
print(np.multiply(a, b))  # Element-wise multiplication
print(np.divide(a, b))  # Element-wise division
print(np.power(a, 2))  # Element-wise exponentiation
```

## 🔄 Aggregation Functions
```python
arr = np.array([1, 2, 3, 4, 5])
print(np.sum(arr))  # Sum of elements
print(np.prod(arr))  # Product of elements
print(np.mean(arr))  # Mean
print(np.std(arr))  # Standard deviation
print(np.var(arr))  # Variance
```

## 📊 Trigonometric Functions
```python
angles = np.array([0, np.pi/2, np.pi])
print(np.sin(angles))  # Sine values
print(np.cos(angles))  # Cosine values
print(np.tan(angles))  # Tangent values
```

## 🏗️ Rounding & Absolute Functions
```python
arr = np.array([-1.7, 1.5, -3.2, 3.8])
print(np.abs(arr))  # Absolute values
print(np.floor(arr))  # Rounding down
print(np.ceil(arr))  # Rounding up
print(np.round(arr))  # Round to nearest integer
```

## 🔄 Bitwise Operations
```python
a = np.array([0, 1, 5])
b = np.array([1, 0, 5])
print(np.bitwise_and(a, b))  # Bitwise AND
print(np.bitwise_or(a, b))  # Bitwise OR
print(np.invert(a))  # Bitwise NOT
```

## 🔥 Comparison Functions
```python
a = np.array([1, 2, 3, 4])
b = np.array([2, 2, 3, 5])
print(np.equal(a, b))  # Element-wise equality
print(np.greater(a, b))  # Greater than
print(np.less(a, b))  # Less than
```

## ⚙️ Custom ufuncs
You can create custom universal functions using `np.frompyfunc()`.
```python
def multiply(x, y):
    return x * y

ufunc_multiply = np.frompyfunc(multiply, 2, 1)
print(ufunc_multiply([1, 2, 3], [4, 5, 6]))
```

## 📜 References
- [NumPy Universal Functions Documentation](https://numpy.org/doc/stable/reference/ufuncs.html)
- [NumPy Mathematical Functions](https://numpy.org/doc/stable/reference/routines.math.html)

🚀 **Keep Exploring NumPy ufuncs for Efficient Computing!**
