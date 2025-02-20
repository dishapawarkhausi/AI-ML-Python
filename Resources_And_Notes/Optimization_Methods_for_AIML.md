# Optimization Methods for AI/ML (with Code)

## 1. Gradient Descent
### Implement Gradient Descent Algorithm:
```python
import numpy as np

def gradient_descent(x, y, lr=0.01, epochs=1000):
    m, b = 0, 0  # Initialize parameters
    n = len(y)
    for _ in range(epochs):
        y_pred = m * x + b
        dm = (-2/n) * sum(x * (y - y_pred))
        db = (-2/n) * sum(y - y_pred)
        m -= lr * dm
        b -= lr * db
    return m, b

x = np.array([1, 2, 3, 4, 5])
y = np.array([2, 2.8, 3.6, 4.5, 5.1])
m, b = gradient_descent(x, y)
print("Optimized m:", m, "Optimized b:", b)
```

## 2. Stochastic Gradient Descent (SGD)
```python
from sklearn.linear_model import SGDRegressor

X = x.reshape(-1, 1)
sgd = SGDRegressor(learning_rate='constant', eta0=0.01, max_iter=1000)
sgd.fit(X, y)
print("SGD Coefficients:", sgd.coef_, "Intercept:", sgd.intercept_)
```

## 3. Newton's Method
```python
from sympy import symbols, diff, solve

x = symbols('x')
f = x**2 - 4*x + 4
derivative = diff(f, x)
second_derivative = diff(derivative, x)
newton_step = x - derivative / second_derivative
solution = solve(newton_step, x)
print("Newton's Method Root:", solution)
```

## 4. Conjugate Gradient Method
```python
from scipy.optimize import minimize

def f(x):
    return x[0]**2 + x[1]**2 + x[0]*x[1] - 6*x[0] - 9*x[1]

x0 = [0, 0]
res = minimize(f, x0, method='CG')
print("Conjugate Gradient Solution:", res.x)
```

## 5. Lagrange Multipliers
```python
from sympy import Eq, solve

x, y, lambda_ = symbols('x y lambda')
f = x**2 + y**2
constraint = x + y - 1
lagrange = f - lambda_ * constraint
df_dx = diff(lagrange, x)
df_dy = diff(lagrange, y)
df_dl = diff(lagrange, lambda_)
solution = solve([df_dx, df_dy, df_dl], (x, y, lambda_))
print("Lagrange Multipliers Solution:", solution)
```

## 6. Bayesian Optimization
```python
from skopt import gp_minimize

def objective(x):
    return (x[0] - 2) ** 2 + (x[1] + 3) ** 2

res = gp_minimize(objective, [(-5.0, 5.0), (-5.0, 5.0)], n_calls=15)
print("Bayesian Optimization Result:", res.x)
```

## 7. Genetic Algorithm
```python
from geneticalgorithm import geneticalgorithm as ga

def f(X):
    return X[0]**2 + X[1]**2

varbound = np.array([[-10, 10], [-10, 10]])
algorithm_param = {'max_num_iteration': 100, 'population_size': 50}
model = ga(function=f, dimension=2, variable_type='real', variable_boundaries=varbound, algorithm_parameters=algorithm_param)
model.run()
```

---
This document now includes Python implementations of key Optimization methods for AI/ML.
