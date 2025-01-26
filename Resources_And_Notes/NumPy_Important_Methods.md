# 📌 NumPy All Methods Cheat Sheet

NumPy provides a vast collection of functions and methods for numerical computing. This guide covers all NumPy methods categorized for quick reference.

## 📥 Import NumPy
```python
import numpy as np
```

---

## 🔹 Array Creation
```python
np.array([1, 2, 3])  # Create a 1D array
np.zeros((2, 3))  # Create a 2x3 array of zeros
np.ones((3, 3))  # Create a 3x3 array of ones
np.full((2, 2), 7)  # Create a 2x2 array filled with 7
np.eye(3)  # Identity matrix of size 3
np.arange(0, 10, 2)  # Create array from 0 to 10 with step 2
np.linspace(0, 1, 5)  # 5 evenly spaced numbers between 0 and 1
np.random.rand(3, 3)  # Create a 3x3 random array
np.random.randn(3, 3)  # Standard normal distribution
np.random.randint(0, 10, (2, 2))  # Random integers in given range
np.random.choice([1, 2, 3, 4], 2)  # Random selection from array
np.meshgrid(x, y)  # Create coordinate matrices
```

---

## 🔹 Array Manipulation
```python
arr = np.array([[1, 2, 3], [4, 5, 6]])
np.reshape(arr, (3, 2))  # Reshape array to 3x2
np.ravel(arr)  # Flatten array to 1D
np.flatten(arr)  # Flatten array
np.transpose(arr)  # Transpose array
np.swapaxes(arr, 0, 1)  # Swap axes
np.expand_dims(arr, axis=0)  # Expand dimensions
np.squeeze(arr)  # Remove single-dimensional entries
np.vstack([arr, arr])  # Vertical stacking
np.hstack([arr, arr])  # Horizontal stacking
np.concatenate([arr, arr], axis=0)  # Concatenate arrays
np.split(arr, 2, axis=0)  # Split array into sub-arrays
np.tile(arr, (2, 2))  # Repeat an array
np.repeat(arr, 2)  # Repeat elements in an array
```

---

## 🔹 Mathematical Operations
```python
np.add(a, b)  # Element-wise addition
np.subtract(a, b)  # Element-wise subtraction
np.multiply(a, b)  # Element-wise multiplication
np.divide(a, b)  # Element-wise division
np.power(a, 2)  # Raise each element to power 2
np.sqrt(a)  # Square root of each element
np.exp(a)  # Exponential of each element
np.log(a)  # Natural log of each element
np.log10(a)  # Base-10 logarithm
np.log2(a)  # Base-2 logarithm
np.cumsum(a)  # Cumulative sum
np.cumprod(a)  # Cumulative product
np.clip(a, min_value, max_value)  # Clip values to a range
```

---

## 🔹 Statistical Functions
```python
np.mean(arr)  # Mean of array
np.median(arr)  # Median of array
np.std(arr)  # Standard deviation
np.var(arr)  # Variance
np.min(arr)  # Minimum value
np.max(arr)  # Maximum value
np.argmin(arr)  # Index of min value
np.argmax(arr)  # Index of max value
np.percentile(arr, 50)  # 50th percentile
np.histogram(arr)  # Compute histogram
```

---

## 🔹 Logical & Comparison Operations
```python
np.equal(a, b)  # Element-wise equality
np.not_equal(a, b)  # Element-wise inequality
np.greater(a, b)  # Element-wise greater than
np.less(a, b)  # Element-wise less than
np.greater_equal(a, b)  # Greater than or equal
np.less_equal(a, b)  # Less than or equal
np.logical_and(a, b)  # Logical AND
np.logical_or(a, b)  # Logical OR
np.logical_not(a)  # Logical NOT
np.isfinite(arr)  # Check if elements are finite
np.isnan(arr)  # Check for NaN values
```

---

## 🔹 Sorting & Searching
```python
np.sort(arr)  # Sort array
np.argsort(arr)  # Get sorted indices
np.argpartition(arr, kth)  # Partial sort
np.argmax(arr)  # Index of max value
np.argmin(arr)  # Index of min value
np.where(arr > 2)  # Indices where condition is met
np.unique(arr)  # Unique elements in array
np.searchsorted(arr, 3)  # Find index for insertion
```

---

## 🔹 Linear Algebra
```python
np.dot(a, b)  # Dot product
np.matmul(a, b)  # Matrix multiplication
np.linalg.inv(matrix)  # Inverse of a matrix
np.linalg.det(matrix)  # Determinant of a matrix
np.linalg.eig(matrix)  # Eigenvalues and eigenvectors
np.linalg.svd(matrix)  # Singular Value Decomposition
np.linalg.norm(matrix)  # Matrix norm
np.linalg.qr(matrix)  # QR decomposition
np.linalg.cholesky(matrix)  # Cholesky decomposition
```

---

## 🔹 Bitwise Operations
```python
np.bitwise_and(a, b)  # Bitwise AND
np.bitwise_or(a, b)  # Bitwise OR
np.bitwise_xor(a, b)  # Bitwise XOR
np.bitwise_not(a)  # Bitwise NOT
np.left_shift(a, 2)  # Left shift
np.right_shift(a, 2)  # Right shift
```

---

## 🔹 File Operations
```python
np.save('data.npy', arr)  # Save array to binary file
np.load('data.npy')  # Load array from binary file
np.savetxt('data.txt', arr)  # Save to text file
np.loadtxt('data.txt')  # Load from text file
np.genfromtxt('data.csv', delimiter=',')  # Load CSV file
```

---

## 📜 References
- [NumPy Documentation](https://numpy.org/doc/stable/)

🚀 **Master NumPy for Efficient Scientific Computing!**
