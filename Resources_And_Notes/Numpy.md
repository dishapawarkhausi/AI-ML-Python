# 📌 NumPy Guide for AI/ML

NumPy (Numerical Python) is a fundamental library for numerical computing in Python. It provides support for large, multi-dimensional arrays and matrices, along with mathematical functions to operate on these arrays.

---

## 📌 Installation
```bash
pip install numpy
```

---

## 🔢 Creating NumPy Arrays
```python
import numpy as np

# Creating an array from a list
arr = np.array([1, 2, 3, 4, 5])

# Creating a 2D array
matrix = np.array([[1, 2, 3], [4, 5, 6]])
```

---

## 📊 Array Operations
```python
# Array shape and size
print(arr.shape)  # (5,)
print(matrix.shape)  # (2,3)
print(arr.size)  # 5

# Reshaping an array
reshaped = arr.reshape((5, 1))
```

---

## 🔄 Array Indexing & Slicing
```python
# Accessing elements
print(arr[0])  # 1
print(matrix[1, 2])  # 6

# Slicing arrays
print(arr[1:4])  # [2, 3, 4]
```

---

## 🔢 Mathematical Operations
```python
# Element-wise operations
arr2 = np.array([10, 20, 30, 40, 50])
print(arr + arr2)  # [11 22 33 44 55]
print(arr * arr2)  # [10 40 90 160 250]

# Mathematical functions
print(np.mean(arr))  # Mean
print(np.std(arr))  # Standard deviation
```

---

## 📏 Special Arrays
```python
zeros = np.zeros((2, 3))  # 2x3 matrix of zeros
ones = np.ones((3, 3))  # 3x3 matrix of ones
identity = np.eye(4)  # 4x4 identity matrix
random_array = np.random.rand(2, 2)  # Random values
```

---

## 🔥 Useful Functions
```python
print(np.linspace(0, 10, 5))  # Evenly spaced numbers
print(np.arange(0, 10, 2))  # Range with step
print(np.dot(arr, arr2))  # Dot product
```

---

## 🏗️ NumPy in AI/ML
NumPy is widely used in AI/ML for:
- Data Preprocessing
- Feature Engineering
- Building Neural Networks
- Handling Large Datasets

---

## 📜 References
- [NumPy Documentation](https://numpy.org/doc/)
- [NumPy Cheat Sheet](https://www.datacamp.com/community/blog/python-numpy-cheat-sheet)

🚀 **Keep Learning & Experimenting!**
