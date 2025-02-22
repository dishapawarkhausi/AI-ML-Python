# SciPy Methods for AI/ML

SciPy is a scientific computing library that provides essential functions for AI and ML applications, including optimization, statistics, signal processing, and linear algebra.

## 1. **Optimization (`scipy.optimize`)**
- `minimize(fun, x0, method='BFGS')` - Minimizes a function using various methods.
- `curve_fit(f, xdata, ydata)` - Fits a function to data.
- `root(fun, x0, method='hybr')` - Finds roots of a function.
- `linprog(c, A_ub, b_ub, method='highs')` - Solves linear programming problems.

## 2. **Linear Algebra (`scipy.linalg`)**
- `inv(A)` - Computes the inverse of a matrix.
- `det(A)` - Computes the determinant of a matrix.
- `eig(A)` - Computes eigenvalues and eigenvectors.
- `svd(A)` - Performs Singular Value Decomposition.
- `solve(A, b)` - Solves a linear system Ax = b.

## 3. **Statistics (`scipy.stats`)**
- `norm.pdf(x, loc, scale)` - Computes the probability density function (PDF) of a normal distribution.
- `norm.cdf(x, loc, scale)` - Computes the cumulative distribution function (CDF) of a normal distribution.
- `t.test_ind(a, b)` - Performs an independent t-test.
- `pearsonr(x, y)` - Computes the Pearson correlation coefficient.
- `zscore(a)` - Computes the z-score for standardization.

## 4. **Sparse Matrices (`scipy.sparse`)**
- `csr_matrix(A)` - Creates a compressed sparse row (CSR) matrix.
- `csc_matrix(A)` - Creates a compressed sparse column (CSC) matrix.
- `coo_matrix(A)` - Creates a coordinate list (COO) sparse matrix.
- `lil_matrix((m, n))` - Creates a list-of-lists sparse matrix.
- `dok_matrix((m, n))` - Creates a dictionary-of-keys sparse matrix.

## 5. **Fourier Transforms (`scipy.fft`)**
- `fft(x)` - Computes the 1D Fast Fourier Transform.
- `ifft(x)` - Computes the Inverse Fast Fourier Transform.
- `fft2(x)` - Computes the 2D FFT.
- `ifft2(x)` - Computes the 2D inverse FFT.

## 6. **Signal Processing (`scipy.signal`)**
- `convolve(a, v, mode='full')` - Computes the convolution of two signals.
- `find_peaks(x)` - Detects peaks in a signal.
- `butter(N, Wn, btype='low')` - Designs a Butterworth filter.
- `lfilter(b, a, x)` - Applies a digital filter to a signal.

## 7. **Interpolation (`scipy.interpolate`)**
- `interp1d(x, y, kind='linear')` - Performs 1D interpolation.
- `griddata(points, values, xi, method='linear')` - Interpolates scattered data.
- `Rbf(x, y, z, function='multiquadric')` - Performs radial basis function interpolation.

## 8. **Integration (`scipy.integrate`)**
- `quad(f, a, b)` - Computes definite integrals.
- `dblquad(f, a, b, gfun, hfun)` - Computes double integrals.
- `simps(y, x)` - Approximates integration using Simpson’s rule.
- `trapz(y, x)` - Approximates integration using the trapezoidal rule.

## 9. **Distance Metrics (`scipy.spatial.distance`)**
- `euclidean(u, v)` - Computes Euclidean distance.
- `cosine(u, v)` - Computes Cosine similarity.
- `jaccard(u, v)` - Computes Jaccard distance.
- `hamming(u, v)` - Computes Hamming distance.

## 10. **Clustering (`scipy.cluster`)**
- `hierarchy.linkage(y, method='single')` - Performs hierarchical clustering.
- `hierarchy.dendrogram(Z)` - Plots a dendrogram for hierarchical clustering.
- `vq.kmeans(data, k)` - Performs k-means clustering.
- `vq.kmeans2(data, k)` - Performs k-means clustering with initial centroids.

## 11. **Miscellaneous (`scipy.misc`)**
- `central_diff_weights(N, ndiv=1)` - Computes weights for central difference approximation.
- `derivative(func, x0, dx=1e-6)` - Computes numerical derivative.

---
This document covers essential SciPy functions useful for AI/ML tasks. Keep updating it with more methods and examples as you explore further!
