# 📌 Advanced Pandas

## 🔹 MultiIndex DataFrames
Pandas allows for hierarchical indexing, making it easy to work with complex datasets.
```python
import pandas as pd
import numpy as np

arrays = [
    ['A', 'A', 'B', 'B'],
    [1, 2, 1, 2]
]
index = pd.MultiIndex.from_arrays(arrays, names=('Letter', 'Number'))
data = np.random.randn(4, 2)
df = pd.DataFrame(data, index=index, columns=['Value1', 'Value2'])
print(df)
```

---

## 🔹 GroupBy Operations
Used to split, apply, and combine data.
```python
df = pd.DataFrame({
    'Category': ['A', 'B', 'A', 'B'],
    'Values': [10, 20, 30, 40]
})
grouped = df.groupby('Category').sum()
print(grouped)
```

---

## 🔹 Merging & Joining DataFrames
Pandas provides powerful methods to combine datasets.
```python
df1 = pd.DataFrame({'ID': [1, 2, 3], 'Name': ['Alice', 'Bob', 'Charlie']})
df2 = pd.DataFrame({'ID': [1, 2, 3], 'Score': [85, 90, 95]})
merged_df = pd.merge(df1, df2, on='ID')
print(merged_df)
```

---

## 🔹 Pivot Tables
Used for summarizing data in a meaningful way.
```python
df = pd.DataFrame({
    'Date': ['2023-01-01', '2023-01-02', '2023-01-01', '2023-01-02'],
    'Category': ['A', 'A', 'B', 'B'],
    'Sales': [100, 150, 200, 250]
})
pivot = df.pivot_table(values='Sales', index='Date', columns='Category', aggfunc='sum')
print(pivot)
```

---

## 🔹 Handling Missing Data
```python
df = pd.DataFrame({'A': [1, np.nan, 3], 'B': [4, 5, np.nan]})
df.fillna(0, inplace=True)
print(df)
```

---

## 🔹 Applying Functions with `apply()`
```python
def square(x):
    return x ** 2

df = pd.DataFrame({'Numbers': [1, 2, 3, 4]})
df['Squared'] = df['Numbers'].apply(square)
print(df)
```

---

🚀 **This guide covers essential advanced Pandas functionalities. Keep exploring!**
