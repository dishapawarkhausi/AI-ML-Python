# AI/ML Mathematics Cheat Sheet

## 1. **Linear Algebra**
- **Matrix Operations**
  - `dot(A, B)`: Matrix multiplication.
  - `transpose(A)`: Transpose of a matrix.
  - `inv(A)`: Inverse of a matrix.
  - `det(A)`: Determinant of a matrix.
  - `eig(A)`: Eigenvalues and eigenvectors.
  - `svd(A)`: Singular Value Decomposition (SVD).
  - `norm(A)`: Norm of a matrix.
  - `trace(A)`: Trace of a matrix.
  - `rank(A)`: Rank of a matrix.
  
## 2. **Calculus**
- **Differentiation**
  - `gradient(f, x)`: Computes gradient.
  - `jacobian(f, x)`: Computes Jacobian matrix.
  - `hessian(f, x)`: Computes Hessian matrix.
  - `diff(f, x)`: Derivative of function.
  - `partial_derivative(f, x, y)`: Partial derivative.
- **Integration**
  - `quad(f, a, b)`: Definite integral.
  - `dblquad(f, a, b, gfun, hfun)`: Double integral.
  - `trapz(y, x)`: Trapezoidal rule for integration.
  - `simps(y, x)`: Simpson’s rule for integration.
  
## 3. **Probability & Statistics**
- **Probability Distributions**
  - `norm.pdf(x, mu, sigma)`: Normal distribution PDF.
  - `norm.cdf(x, mu, sigma)`: Normal distribution CDF.
  - `poisson.pmf(k, lambda)`: Poisson distribution.
  - `binom.pmf(k, n, p)`: Binomial distribution.
  - `expon.pdf(x, lambda)`: Exponential distribution.
- **Descriptive Statistics**
  - `mean(x)`: Computes mean.
  - `median(x)`: Computes median.
  - `mode(x)`: Computes mode.
  - `variance(x)`: Computes variance.
  - `std(x)`: Computes standard deviation.
  - `corrcoef(X, Y)`: Correlation coefficient.
  - `zscore(x)`: Z-score normalization.
  
## 4. **Optimization**
- `minimize(f, x0, method)`: General function minimization.
- `linprog(c, A_ub, b_ub)`: Linear programming.
- `root(f, x0)`: Finds roots of a function.
- `curve_fit(f, xdata, ydata)`: Fits a function to data.
- `gradient_descent(f, lr, epochs)`: Gradient descent optimization.
  
## 5. **Distance Metrics**
- `euclidean(u, v)`: Euclidean distance.
- `manhattan(u, v)`: Manhattan distance.
- `minkowski(u, v, p)`: Minkowski distance.
- `cosine(u, v)`: Cosine similarity.
- `jaccard(u, v)`: Jaccard similarity.
- `hamming(u, v)`: Hamming distance.
  
## 6. **Transformations**
- **Fourier Transform**
  - `fft(x)`: Fast Fourier Transform.
  - `ifft(x)`: Inverse Fast Fourier Transform.
- **Logarithms and Exponentials**
  - `log(x)`: Natural logarithm.
  - `log10(x)`: Base-10 logarithm.
  - `log2(x)`: Base-2 logarithm.
  - `exp(x)`: Exponential function.
  - `sigmoid(x)`: Sigmoid function.
  - `softmax(x)`: Softmax activation function.
  
## 7. **Graph Theory**
- `shortest_path(graph, source)`: Finds shortest path.
- `adjacency_matrix(graph)`: Computes adjacency matrix.
- `pagerank(graph)`: Computes PageRank scores.
- `connected_components(graph)`: Finds connected components.
- `degree_centrality(graph)`: Computes node centrality.
  
## 8. **Miscellaneous**
- `factorial(n)`: Computes factorial of n.
- `gamma(x)`: Gamma function.
- `beta(x, y)`: Beta function.
- `sigmoid(x)`: Computes sigmoid activation.
- `relu(x)`: Rectified Linear Unit activation.
- `tanh(x)`: Hyperbolic tangent function.
  
---
This cheat sheet provides an overview of key mathematical methods for AI/ML. Keep updating it with more concepts and examples as you explore further!
