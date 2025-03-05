# Python `statistics` Module Cheat Sheet

## 1. **Importing the Statistics Module**
```python
import statistics
```

## 2. **Measures of Central Tendency**
### Mean (Average)
```python
print(statistics.mean([1, 2, 3, 4, 5]))  # 3.0
```
### Median (Middle Value)
```python
print(statistics.median([1, 3, 5, 7, 9]))  # 5
print(statistics.median([1, 2, 3, 4, 5, 6]))  # 3.5
```
### Mode (Most Common Value)
```python
print(statistics.mode([1, 2, 2, 3, 3, 3, 4]))  # 3
```

## 3. **Measures of Dispersion**
### Standard Deviation (Spread of Data)
```python
print(statistics.stdev([1, 2, 3, 4, 5]))  # Standard deviation
```
### Variance (Square of Standard Deviation)
```python
print(statistics.variance([1, 2, 3, 4, 5]))  # Variance
```
### Median Absolute Deviation (MAD)
```python
print(statistics.median_high([1, 2, 3, 4, 5]))  # 3 (high median)
print(statistics.median_low([1, 2, 3, 4, 5]))  # 3 (low median)
```

## 4. **Other Statistical Functions**
### Harmonic Mean
```python
print(statistics.harmonic_mean([1, 2, 3]))  # 1.6363
```
### Geometric Mean
```python
print(statistics.geometric_mean([1, 10, 100]))  # 10.0
```
### Quantiles
```python
print(statistics.quantiles([1, 2, 3, 4, 5], n=4))  # Quartiles
```

---
This cheat sheet covers essential Python `statistics` module functions. 🚀
