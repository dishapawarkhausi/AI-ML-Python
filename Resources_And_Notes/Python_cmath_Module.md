# Python `cmath` Module Cheat Sheet

## 1. **Importing the cmath Module**
The `cmath` module provides mathematical functions for complex numbers.
```python
import cmath
```

## 2. **Basic Operations on Complex Numbers**
### Creating a Complex Number
```python
z = complex(3, 4)  # 3 + 4j
print(z)
```
### Getting Real and Imaginary Parts
```python
print(z.real)  # 3.0
print(z.imag)  # 4.0
```
### Conjugate of a Complex Number
```python
print(z.conjugate())  # 3 - 4j
```

## 3. **Magnitude and Phase**
### Absolute Value (Magnitude)
```python
print(abs(z))  # 5.0
```
### Phase Angle
```python
print(cmath.phase(z))  # 0.927 radians
```
### Convert to Polar Form
```python
r, phi = cmath.polar(z)
print(r, phi)  # (5.0, 0.927)
```
### Convert from Polar to Rectangular Form
```python
print(cmath.rect(r, phi))  # (3+4j)
```

## 4. **Exponential and Logarithmic Functions**
### Exponential of a Complex Number
```python
print(cmath.exp(z))
```
### Natural Logarithm
```python
print(cmath.log(z))
```
### Logarithm with Custom Base
```python
print(cmath.log(z, 10))
```

## 5. **Trigonometric Functions**
### Sine, Cosine, and Tangent
```python
print(cmath.sin(z))
print(cmath.cos(z))
print(cmath.tan(z))
```
### Inverse Trigonometric Functions
```python
print(cmath.asin(z))
print(cmath.acos(z))
print(cmath.atan(z))
```

## 6. **Hyperbolic Functions**
### Hyperbolic Sine, Cosine, Tangent
```python
print(cmath.sinh(z))
print(cmath.cosh(z))
print(cmath.tanh(z))
```
### Inverse Hyperbolic Functions
```python
print(cmath.asinh(z))
print(cmath.acosh(z))
print(cmath.atanh(z))
```

---
This cheat sheet covers essential Python `cmath` module functions for working with complex numbers. 🚀
