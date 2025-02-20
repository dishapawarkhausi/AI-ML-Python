# Linear Algebra for AI/ML (with Code)

## 1. Vectors and Operations
### Vector Addition and Scalar Multiplication:
```python
import numpy as np

v1 = np.array([1, 2, 3])
v2 = np.array([4, 5, 6])
scalar = 3

print("Vector Addition:", v1 + v2)
print("Scalar Multiplication:", scalar * v1)
```

## 2. Matrices and Operations
### Matrix Addition, Multiplication, and Transposition:
```python
A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])

print("Matrix Addition:\n", A + B)
print("Matrix Multiplication:\n", np.dot(A, B))
print("Matrix Transposition:\n", A.T)
```

## 3. Determinants and Inverse
### Compute Determinant and Inverse of a Matrix:
```python
A = np.array([[4, 7], [2, 6]])

det_A = np.linalg.det(A)
inv_A = np.linalg.inv(A)
print("Determinant:", det_A)
print("Inverse:\n", inv_A)
```

## 4. Eigenvalues and Eigenvectors
### Compute Eigenvalues and Eigenvectors:
```python
A = np.array([[3, 1], [0, 2]])

eigenvalues, eigenvectors = np.linalg.eig(A)
print("Eigenvalues:", eigenvalues)
print("Eigenvectors:\n", eigenvectors)
```

## 5. Singular Value Decomposition (SVD)
### Perform SVD:
```python
A = np.array([[1, 2], [3, 4], [5, 6]])

U, S, Vt = np.linalg.svd(A)
print("U:\n", U)
print("Singular Values:", S)
print("Vt:\n", Vt)
```

## 6. Principal Component Analysis (PCA)
### Reduce Dimensions Using PCA:
```python
from sklearn.decomposition import PCA

X = np.array([[2.5, 2.4], [0.5, 0.7], [2.2, 2.9], [1.9, 2.2]])
pca = PCA(n_components=1)
X_reduced = pca.fit_transform(X)
print("Reduced Data:\n", X_reduced)
```

## 7. Least Squares Regression
### Solve Using Least Squares:
```python
A = np.array([[1, 1], [1, 2], [1, 3]])
y = np.array([2, 2.5, 3.5])

coefficients = np.linalg.lstsq(A, y, rcond=None)[0]
print("Regression Coefficients:", coefficients)
```

---
This document now includes Python implementations of key Linear Algebra concepts for AI/ML.
