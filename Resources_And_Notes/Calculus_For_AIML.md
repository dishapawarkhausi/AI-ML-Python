# Calculus for AI/ML (with Code)

## 1. Limits and Derivatives
### Compute the Derivative of a Function:
```python
import sympy as sp

x = sp.symbols('x')
f = x**2 + 3*x + 5
derivative_f = sp.diff(f, x)
print("Derivative:", derivative_f)
```

## 2. Partial Derivatives
### Compute Partial Derivatives:
```python
x, y = sp.symbols('x y')
f = x**2 + y**2
partial_x = sp.diff(f, x)
partial_y = sp.diff(f, y)
print("Partial Derivative w.r.t x:", partial_x)
print("Partial Derivative w.r.t y:", partial_y)
```

## 3. Gradient and Hessian
### Compute the Gradient and Hessian Matrix:
```python
from sympy import Matrix

f = x**2 + 3*y**2

grad = Matrix([sp.diff(f, var) for var in (x, y)])
hessian = grad.jacobian([x, y])
print("Gradient:\n", grad)
print("Hessian Matrix:\n", hessian)
```

## 4. Integration
### Compute the Integral of a Function:
```python
integral_f = sp.integrate(f, x)
print("Integral:", integral_f)
```

## 5. Double Integration
### Compute Double Integral:
```python
double_integral = sp.integrate(sp.integrate(f, x), y)
print("Double Integral:", double_integral)
```

## 6. Chain Rule
### Compute Chain Rule for Composite Function:
```python
g = sp.sin(x)
f = x**2
df_dx = sp.diff(f, x)
dg_dx = sp.diff(g, x)
chain_rule_result = df_dx * dg_dx
print("Chain Rule Result:", chain_rule_result)
```

## 7. Taylor Series Approximation
### Compute Taylor Series Expansion:
```python
taylor_series = sp.series(sp.exp(x), x, 0, 5)
print("Taylor Series Expansion:\n", taylor_series)
```

## 8. Optimization
### Find Critical Points:
```python
critical_points = sp.solve(sp.diff(f, x), x)
print("Critical Points:", critical_points)
```

---
This document now includes Python implementations of key Calculus concepts for AI/ML.
