# Linear Algebra for AI/ML

## 1. Vectors
### Definition:
A vector is an ordered list of numbers, often represented as a column or row matrix.

### Operations:
- **Addition**: \( \mathbf{a} + \mathbf{b} \)
- **Subtraction**: \( \mathbf{a} - \mathbf{b} \)
- **Scalar Multiplication**: \( c \mathbf{a} \)
- **Dot Product**: \( \mathbf{a} \cdot \mathbf{b} = \sum a_i b_i \)
- **Cross Product** (for 3D vectors): \( \mathbf{a} \times \mathbf{b} \)
- **Norm (Magnitude)**: \( ||\mathbf{a}|| = \sqrt{\sum a_i^2} \)

## 2. Matrices
### Definition:
A matrix is a 2D array of numbers arranged in rows and columns.

### Operations:
- **Addition/Subtraction**: \( A + B \) or \( A - B \)
- **Scalar Multiplication**: \( cA \)
- **Matrix Multiplication**: \( AB \) (dot product of rows and columns)
- **Transpose**: \( A^T \) (flips rows & columns)
- **Determinant**: \( \det(A) \) (used to determine invertibility)
- **Inverse**: \( A^{-1} \) (exists if \( \det(A) \neq 0 \))
- **Rank**: Number of linearly independent rows/columns
- **Trace**: Sum of diagonal elements \( \text{tr}(A) \)

## 3. Special Matrices
- **Identity Matrix** \( I \): Diagonal elements are 1, others are 0.
- **Diagonal Matrix**: Non-diagonal elements are zero.
- **Orthogonal Matrix**: \( A^T A = I \).
- **Symmetric Matrix**: \( A^T = A \).
- **Singular Matrix**: \( \det(A) = 0 \), non-invertible.

## 4. Eigenvalues & Eigenvectors
### Definition:
For a matrix \( A \), an eigenvector \( \mathbf{v} \) and eigenvalue \( \lambda \) satisfy:
\[ A\mathbf{v} = \lambda \mathbf{v} \]

### Finding Eigenvalues:
Solve \( \det(A - \lambda I) = 0 \).

### Finding Eigenvectors:
Solve \( (A - \lambda I) \mathbf{v} = 0 \).

## 5. Singular Value Decomposition (SVD)
\[ A = U \Sigma V^T \]
Where:
- \( U \) & \( V \) are orthogonal matrices.
- \( \Sigma \) is a diagonal matrix of singular values.

## 6. Principal Component Analysis (PCA)
PCA is used for dimensionality reduction using eigenvalues/eigenvectors.
### Steps:
1. Standardize data.
2. Compute covariance matrix.
3. Compute eigenvalues/eigenvectors.
4. Select top k components.
5. Transform data.

## 7. Vector Spaces & Basis
- **Span**: Set of all linear combinations of vectors.
- **Basis**: Minimal set of linearly independent vectors that span a space.
- **Dimension**: Number of basis vectors.

## 8. Norms & Distance Metrics
- **L1 Norm (Manhattan Distance)**: \( ||x||_1 = \sum |x_i| \)
- **L2 Norm (Euclidean Distance)**: \( ||x||_2 = \sqrt{\sum x_i^2} \)
- **Frobenius Norm** (for matrices): \( ||A||_F = \sqrt{\sum A_{ij}^2} \)

## 9. Linear Transformations
A function \( f: \mathbb{R}^n \to \mathbb{R}^m \) is linear if:
- \( f(a + b) = f(a) + f(b) \)
- \( f(ca) = c f(a) \)

## 10. Systems of Linear Equations
Solving \( Ax = b \):
- **Gaussian Elimination**
- **LU Decomposition**
- **Matrix Inversion** (if \( A \) is invertible)
- **Least Squares** (for overdetermined systems)

## 11. Applications in AI/ML
- **Feature Engineering**: PCA for dimensionality reduction.
- **Neural Networks**: Weight matrices and transformations.
- **Computer Vision**: Image transformations using matrices.
- **Recommendation Systems**: SVD for latent factor analysis.
- **Optimization**: Gradient descent in vector spaces.

---
This document serves as a reference for essential linear algebra concepts required in AI/ML. Keep updating with practical examples!
