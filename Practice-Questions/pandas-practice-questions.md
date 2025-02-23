# Pandas Coding Practice Questions

## 👉 1. Basic Pandas Questions

1. Import Pandas and print its version.
2. Create a Pandas Series from a Python list `[10, 20, 30, 40, 50]`.
3. Create a Pandas Series with custom index `['a', 'b', 'c', 'd', 'e']` for values `[5, 10, 15, 20, 25]`.
4. Create a Pandas DataFrame from a dictionary:
   ```python
   data = {'Name': ['Alice', 'Bob', 'Charlie'],
           'Age': [25, 30, 35],
           'Salary': [50000, 60000, 70000]}
   ```
5. Read a CSV file named **"data.csv"** into a Pandas DataFrame.
6. Display the first 7 rows of a DataFrame.
7. Display the last 5 rows of a DataFrame.
8. Get the number of rows and columns in a DataFrame.
9. Check the data types of each column.
10. Rename the column `"Salary"` to `"Income"`.
11. Drop a column `"Age"` from the DataFrame.
12. Drop all rows containing missing values.
13. Fill all missing values with `0`.
14. Convert a column `"Salary"` to integer type.
15. Sort the DataFrame by `"Age"` in descending order.
16. Reset the index of a DataFrame.
17. Set the `"Name"` column as the index.
18. Check for duplicate rows in a DataFrame.
19. Remove duplicate rows from a DataFrame.
20. Save the DataFrame as `"output.csv"`.

---

## 👉 2. Intermediate Pandas Questions

21. Select only the `"Name"` and `"Salary"` columns from the DataFrame.
22. Select rows where `"Age"` is greater than 30.
23. Select rows where `"Salary"` is between 50000 and 65000.
24. Use `.loc[]` to select rows where `"Age"` is 30 and `"Salary"` is 60000.
25. Use `.iloc[]` to select the first 3 rows and 2 columns.
26. Compute the mean salary of all employees.
27. Find the median age of employees.
28. Group the DataFrame by `"Age"` and calculate the average salary.
29. Create a pivot table with `"Age"` as index and `"Salary"` as values.
30. Apply a lambda function to increase all salaries by 10%.
31. Replace all salaries below 60000 with `"Low"`.
32. Merge two DataFrames on a common `"Employee_ID"` column.
33. Concatenate two DataFrames vertically.
34. Convert the `"Hire_Date"` column to datetime format.
35. Extract the year, month, and day from a datetime column.
36. Create a new column `"Bonus"` which is 10% of `"Salary"`.
37. Convert the categorical column `"Department"` into numeric values.
38. Replace all occurrences of `"Manager"` in a column with `"Team Lead"`.
39. Save the DataFrame to an Excel file `"data.xlsx"`.
40. Read an Excel file into a DataFrame.

---

## 👉 3. Advanced Pandas Questions

41. Load a large dataset efficiently using Pandas.
42. Use `.query()` to filter rows where `"Salary"` is greater than `65000`.
43. Identify and remove outliers in a numerical column.
44. Compute a rolling mean with a window size of 3 for the `"Salary"` column.
45. Pivot the DataFrame to reshape it.
46. Convert a JSON dataset into a Pandas DataFrame.
47. Optimize memory usage by changing data types in a large DataFrame.
48. Use multi-indexing with two columns.
49. Perform a time series analysis by setting `"Date"` as the index.
50. Write a function that normalizes a numerical column and apply it to `"Salary"`.

---

### ✅ **How to Use**
- Try solving these **50 hands-on Pandas coding problems**.
- Test each question by writing a Python script or Jupyter Notebook.
- Experiment with **real datasets** to enhance your skills!

Happy coding! 🚀
