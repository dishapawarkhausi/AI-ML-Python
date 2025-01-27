# 📌 Introduction to Pandas

Pandas is a powerful open-source data analysis and manipulation library for Python. It provides data structures and functions needed to efficiently analyze structured data.

## 🔹 Why Use Pandas?
- Easy handling of missing data
- Powerful data manipulation using DataFrame and Series
- Support for loading data from various formats (CSV, Excel, JSON, SQL, etc.)
- Efficient handling of large datasets
- Built-in data visualization support

---

## 📥 Installing Pandas
```python
pip install pandas
```

---

## 🔹 Importing Pandas
```python
import pandas as pd
```

---

## 🔹 Core Data Structures in Pandas
### 1️⃣ Series (1D Data)
```python
s = pd.Series([10, 20, 30, 40])
print(s)
```

### 2️⃣ DataFrame (2D Data)
```python
data = {'Name': ['Alice', 'Bob', 'Charlie'], 'Age': [25, 30, 35]}
df = pd.DataFrame(data)
print(df)
```

---

## 🔹 Loading Data
```python
df = pd.read_csv('data.csv')  # Load CSV file
df = pd.read_excel('data.xlsx')  # Load Excel file
df = pd.read_json('data.json')  # Load JSON file
```

---

## 🔹 Basic DataFrame Operations
```python
print(df.head())  # First 5 rows
print(df.tail())  # Last 5 rows
print(df.info())  # Data types and memory usage
print(df.describe())  # Summary statistics
```

---

🚀 **Stay tuned for more advanced Pandas functions!**
