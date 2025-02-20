# Probability & Statistics for AI/ML (with Code)

## 1. Probability Basics
### Bayes’ Theorem:
```python
import numpy as np

def bayes_theorem(prior_A, prob_B_given_A, prob_B):
    return (prob_B_given_A * prior_A) / prob_B

# Example
prior_A = 0.3  # P(A)
prob_B_given_A = 0.7  # P(B|A)
prob_B = 0.5  # P(B)

posterior_A_given_B = bayes_theorem(prior_A, prob_B_given_A, prob_B)
print("P(A|B) =", posterior_A_given_B)
```

## 2. Random Variables & Distributions
### Normal Distribution:
```python
import matplotlib.pyplot as plt
from scipy.stats import norm

x = np.linspace(-5, 5, 100)
y = norm.pdf(x, loc=0, scale=1)

plt.plot(x, y, label="Normal Distribution")
plt.legend()
plt.show()
```

## 3. Descriptive Statistics
### Mean, Median, and Standard Deviation:
```python
import numpy as np

data = [10, 20, 30, 40, 50]
print("Mean:", np.mean(data))
print("Median:", np.median(data))
print("Standard Deviation:", np.std(data))
```

## 4. Inferential Statistics
### Hypothesis Testing (t-test):
```python
from scipy.stats import ttest_ind

group1 = [12, 14, 15, 16, 18]
group2 = [22, 24, 25, 26, 28]
t_stat, p_value = ttest_ind(group1, group2)
print("t-statistic:", t_stat)
print("p-value:", p_value)
```

## 5. Correlation & Regression
### Correlation:
```python
import numpy as np

x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]
print("Correlation Coefficient:", np.corrcoef(x, y)[0, 1])
```

### Linear Regression:
```python
import numpy as np
from sklearn.linear_model import LinearRegression

X = np.array([1, 2, 3, 4, 5]).reshape(-1, 1)
y = np.array([2, 4, 6, 8, 10])

model = LinearRegression()
model.fit(X, y)
print("Slope:", model.coef_[0])
print("Intercept:", model.intercept_)
```

## 6. Probability Distributions in AI/ML
### Sampling from a Poisson Distribution:
```python
import numpy as np
import matplotlib.pyplot as plt

samples = np.random.poisson(lam=3, size=1000)
plt.hist(samples, bins=15, density=True, alpha=0.6, color='g')
plt.show()
```

## 7. Bayesian Statistics
### Naïve Bayes Classifier:
```python
from sklearn.naive_bayes import GaussianNB
import numpy as np

X = np.array([[1, 2], [2, 3], [3, 4], [4, 5]])
y = np.array([0, 0, 1, 1])

model = GaussianNB()
model.fit(X, y)
print("Prediction:", model.predict([[2.5, 3.5]]))
```

## 8. Statistical Learning
### Maximum Likelihood Estimation (MLE):
```python
import numpy as np
from scipy.stats import norm

data = np.array([2.1, 2.5, 3.0, 3.2, 4.0])
mean_MLE = np.mean(data)
std_MLE = np.std(data)
print("MLE Mean:", mean_MLE)
print("MLE Standard Deviation:", std_MLE)
```

---
This document now includes Python implementations of key Probability & Statistics concepts for AI/ML.
