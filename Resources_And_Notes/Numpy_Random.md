# 🎲 NumPy Random Module Guide

The `numpy.random` module provides various functions to generate random numbers, arrays, and distributions, essential for AI/ML applications such as data augmentation, simulations, and probabilistic modeling.

---

## 📌 Importing NumPy Random
```python
import numpy as np
```

---

## 🔢 Generating Random Numbers
```python
print(np.random.rand(3))  # Uniform distribution between 0 and 1
print(np.random.randn(3))  # Standard normal distribution
print(np.random.randint(1, 10, 5))  # Random integers between 1 and 10
```

---

## 🎲 Random Sampling
```python
arr = np.array([10, 20, 30, 40, 50])
print(np.random.choice(arr))  # Random selection from an array
```

---

## 🔄 Shuffling & Permutation
```python
np.random.shuffle(arr)  # In-place shuffling
print(arr)

print(np.random.permutation(arr))  # Returns a shuffled copy
```

---

## 📊 Probability Distributions
```python
print(np.random.normal(0, 1, 5))  # Normal distribution (mean=0, std=1)
print(np.random.uniform(1, 10, 5))  # Uniform distribution between 1 and 10
print(np.random.poisson(3, 5))  # Poisson distribution with lambda=3
```

---

## 🏗️ Setting Seed for Reproducibility
```python
np.random.seed(42)
print(np.random.rand(3))  # Same output every time
```

---

## 📜 References
- [NumPy Random Documentation](https://numpy.org/doc/stable/reference/random/index.html)
- [Random Sampling in NumPy](https://numpy.org/doc/stable/reference/random/generated/numpy.random.choice.html)

🚀 **Experiment & Explore NumPy Random!**
