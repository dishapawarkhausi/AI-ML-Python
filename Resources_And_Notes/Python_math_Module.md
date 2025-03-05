# Python `math` Module Cheat Sheet

## 1. **Importing the Math Module**
The `math` module provides mathematical functions for performing calculations.
```python
import math
```

## 2. **Basic Mathematical Functions**
### Square Root
Finds the square root of a given number.
```python
print(math.sqrt(25))  # 5.0
```
### Power
Computes the power of a number.
```python
print(math.pow(2, 3))  # 8.0 (2^3)
```
Computes the exponential of a number (e^x).
```python
print(math.exp(2))  # e^2
```
### Absolute Value
Returns the absolute (positive) value of a number.
```python
print(math.fabs(-10))  # 10.0
```
### Factorial
Finds the factorial of a number.
```python
print(math.factorial(5))  # 120 (5!)
```

## 3. **Rounding Functions**
### Floor (Round Down)
Rounds a number down to the nearest integer.
```python
print(math.floor(4.9))  # 4
```
### Ceil (Round Up)
Rounds a number up to the nearest integer.
```python
print(math.ceil(4.1))  # 5
```

## 4. **Trigonometric Functions**
### Sine, Cosine, Tangent
Calculates the sine, cosine, and tangent of an angle in degrees.
```python
print(math.sin(math.radians(30)))  # 0.5
print(math.cos(math.radians(60)))  # 0.5
print(math.tan(math.radians(45)))  # 1.0
```
### Inverse Trigonometric Functions
Finds the inverse sine (arcsin) of a given value and converts it to degrees.
```python
print(math.degrees(math.asin(0.5)))  # 30.0
```
### Pi and Euler’s Number
Returns the values of Pi (π) and Euler’s number (e).
```python
print(math.pi)  # 3.141592653589793
print(math.e)  # 2.718281828459045
```

## 5. **Logarithmic Functions**
### Natural Logarithm (Base e)
Computes the natural logarithm (log base e) of a number.
```python
print(math.log(10))  # 2.302585092994046
```
### Logarithm with Custom Base
Finds the logarithm of a number with a specified base.
```python
print(math.log(100, 10))  # 2.0 (log base 10 of 100)
```

## 6. **GCD and LCM**
### Greatest Common Divisor (GCD)
Finds the greatest common divisor of two numbers.
```python
print(math.gcd(48, 18))  # 6
```
### Least Common Multiple (LCM)
Computes the least common multiple of two numbers using GCD.
```python
import math
from functools import reduce

def lcm(a, b):
    return abs(a * b) // math.gcd(a, b)

print(lcm(12, 18))  # 36
```

---
This cheat sheet covers essential Python `math` module functions with explanations. 🚀
