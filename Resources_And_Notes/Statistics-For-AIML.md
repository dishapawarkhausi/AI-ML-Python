# Statistics for AI/ML - All Important Methods

## 1. **Descriptive Statistics**
- **Measures of Central Tendency:**
  - `mean(x)`: Arithmetic mean of data.
  - `median(x)`: Middle value in sorted data.
  - `mode(x)`: Most frequently occurring value.
- **Measures of Dispersion:**
  - `variance(x)`: Variance of data.
  - `std(x)`: Standard deviation.
  - `range(x)`: Difference between max and min.
  - `iqr(x)`: Interquartile range (Q3 - Q1).
- **Correlation & Covariance:**
  - `corrcoef(X, Y)`: Pearson correlation coefficient.
  - `cov(X, Y)`: Covariance matrix.
  - `spearmanr(X, Y)`: Spearman rank correlation.
  - `kendalltau(X, Y)`: Kendall’s tau correlation.

## 2. **Probability Distributions**
- **Discrete Distributions:**
  - `binom.pmf(k, n, p)`: Binomial distribution.
  - `poisson.pmf(k, lambda)`: Poisson distribution.
  - `geom.pmf(k, p)`: Geometric distribution.
- **Continuous Distributions:**
  - `norm.pdf(x, mu, sigma)`: Normal (Gaussian) PDF.
  - `norm.cdf(x, mu, sigma)`: Normal CDF.
  - `expon.pdf(x, lambda)`: Exponential distribution.
  - `uniform.pdf(x, a, b)`: Uniform distribution.
  - `gamma.pdf(x, alpha, beta)`: Gamma distribution.

## 3. **Inferential Statistics**
- **Hypothesis Testing:**
  - `ttest_ind(A, B)`: Independent t-test.
  - `ttest_rel(A, B)`: Paired t-test.
  - `chi2_contingency(table)`: Chi-square test.
  - `anova1way(*groups)`: One-way ANOVA.
  - `anova2way(data)`: Two-way ANOVA.
- **Confidence Intervals:**
  - `conf_int(x, confidence)`: Computes confidence interval.
- **Resampling Methods:**
  - `bootstrap(x, n_samples)`: Bootstrap resampling.
  - `jackknife(x)`: Jackknife resampling.

## 4. **Regression Analysis**
- **Linear Regression:**
  - `linregress(X, Y)`: Simple linear regression.
  - `ols(formula, data)`: Ordinary least squares (OLS).
- **Multiple & Polynomial Regression:**
  - `polyfit(X, Y, degree)`: Polynomial regression.
  - `ridge(X, Y, alpha)`: Ridge regression.
  - `lasso(X, Y, alpha)`: Lasso regression.
- **Logistic Regression:**
  - `logit.fit(X, Y)`: Logistic regression.

## 5. **Bayesian Statistics**
- **Bayes Theorem:**
  - `posterior = (prior * likelihood) / evidence`
- **Bayesian Inference:**
  - `beta(a, b)`: Beta distribution (used in Bayesian updating).
  - `dirichlet(alpha)`: Dirichlet distribution.

## 6. **Statistical Learning & Feature Selection**
- **Feature Selection Methods:**
  - `f_classif(X, Y)`: ANOVA F-value.
  - `mutual_info_classif(X, Y)`: Mutual information.
- **Dimensionality Reduction:**
  - `pca.fit(X)`: Principal Component Analysis (PCA).
  - `lda.fit(X, Y)`: Linear Discriminant Analysis (LDA).

## 7. **Outlier Detection & Robust Statistics**
- **Outlier Detection:**
  - `zscore(X)`: Z-score method.
  - `iqr(X)`: Interquartile range method.
  - `lof.fit(X)`: Local Outlier Factor (LOF).
  - `isolation_forest.fit(X)`: Isolation Forest.

## 8. **Time Series Analysis**
- **Basic Statistics for Time Series:**
  - `autocorr(X)`: Autocorrelation function.
  - `pacf(X)`: Partial autocorrelation function.
- **Forecasting Models:**
  - `arima.fit(X)`: ARIMA model.
  - `holt_winters.fit(X)`: Holt-Winters method.
  - `prophet.fit(X)`: Facebook Prophet for forecasting.

---
This document covers essential statistics methods for AI/ML. Keep updating it with more insights and applications as you explore further!
