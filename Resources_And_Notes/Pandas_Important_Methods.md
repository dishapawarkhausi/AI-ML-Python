# 📌 Pandas All Important Methods

## 🔹 DataFrame Creation
```python
import pandas as pd
import numpy as np

df = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6]})
print(df)
```

---

## 🔹 Viewing Data
```python
print(df.head())   # First 5 rows
print(df.tail())   # Last 5 rows
print(df.info())   # Summary of DataFrame
print(df.describe())  # Statistical summary
print(df.shape)   # Shape of DataFrame
print(df.columns)  # List of columns
print(df.index)  # List of index values
```

---

## 🔹 Selecting Data
```python
print(df['A'])   # Select single column
print(df[['A', 'B']])  # Select multiple columns
print(df.loc[0])  # Select row by label
print(df.iloc[0])  # Select row by index
print(df.loc[0, 'A'])  # Select specific value
print(df.iloc[0, 1])  # Select value by index
```

---

## 🔹 Filtering Data
```python
print(df[df['A'] > 1])  # Rows where column A is greater than 1
print(df.query("A > 1"))  # Query-based filtering
```

---

## 🔹 Sorting Data
```python
print(df.sort_values(by='A', ascending=False))  # Sort by column A descending
print(df.sort_index())  # Sort by index
```

---

## 🔹 Handling Missing Data
```python
df.fillna(0, inplace=True)  # Fill missing values with 0
df.dropna(inplace=True)  # Remove missing values
df.isnull().sum()  # Check for null values
```

---

## 🔹 Adding & Removing Columns
```python
df['C'] = df['A'] + df['B']  # Create a new column
df.drop('C', axis=1, inplace=True)  # Drop column C
```

---

## 🔹 Adding & Removing Rows
```python
df.loc[3] = [7, 8]  # Add a new row
df.drop(3, axis=0, inplace=True)  # Remove a row by index
```

---

## 🔹 Grouping Data
```python
grouped = df.groupby('A').sum()
print(grouped)
```

---

## 🔹 Merging & Joining
```python
df1 = pd.DataFrame({'ID': [1, 2], 'Name': ['Alice', 'Bob']})
df2 = pd.DataFrame({'ID': [1, 2], 'Score': [85, 90]})
merged_df = pd.merge(df1, df2, on='ID')
print(merged_df)
```

---

## 🔹 Concatenation
```python
df3 = pd.concat([df1, df2], axis=0)
print(df3)
```

---

## 🔹 Pivot Table
```python
df = pd.DataFrame({
    'Category': ['A', 'B', 'A', 'B'],
    'Values': [10, 20, 30, 40]
})
pivot = df.pivot_table(values='Values', index='Category', aggfunc=np.mean)
print(pivot)
```

---

## 🔹 Apply Function
```python
def square(x):
    return x ** 2

df['Squared'] = df['A'].apply(square)
print(df)
```

---

## 🔹 Handling Duplicates
```python
df.drop_duplicates(inplace=True)  # Remove duplicate rows
print(df.duplicated())  # Check for duplicates
```

---

## 🔹 Changing Data Types
```python
df['A'] = df['A'].astype(float)  # Convert column A to float
```

---

## 🔹 String Operations
```python
df['Name'] = df['Name'].str.upper()  # Convert names to uppercase
print(df['Name'].str.contains('A'))  # Check if names contain 'A'
```

---

## 🔹 Date & Time Handling
```python
df['Date'] = pd.to_datetime(['2023-01-01', '2023-01-02'])
print(df['Date'].dt.day)  # Extract day from date
```

---

## 🔹 Exporting Data
```python
df.to_csv('output.csv', index=False)  # Save DataFrame to CSV
df.to_excel('output.xlsx', index=False)  # Save DataFrame to Excel
```

---

🚀 **This guide covers all essential Pandas methods. Keep practicing!**
