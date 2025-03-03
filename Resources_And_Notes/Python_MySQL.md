# Python MySQL - All Important Methods

## 1. **Installing MySQL Connector**
```sh
pip install mysql-connector-python
```

## 2. **Connecting to MySQL Database**
```python
import mysql.connector

conn = mysql.connector.connect(
    host="localhost",
    user="your_username",
    password="your_password",
    database="your_database"
)
cursor = conn.cursor()
```

## 3. **Creating a Database**
```python
cursor.execute("CREATE DATABASE mydatabase")
```

## 4. **Showing Databases**
```python
cursor.execute("SHOW DATABASES")
for db in cursor:
    print(db)
```

## 5. **Creating a Table**
```python
cursor.execute("""
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255),
    email VARCHAR(255)
)
""")
```

## 6. **Inserting Data into a Table**
```python
sql = "INSERT INTO users (name, email) VALUES (%s, %s)"
values = ("John Doe", "john@example.com")
cursor.execute(sql, values)
conn.commit()
print(cursor.rowcount, "record inserted.")
```

## 7. **Selecting Data from a Table**
```python
cursor.execute("SELECT * FROM users")
result = cursor.fetchall()
for row in result:
    print(row)
```

## 8. **Selecting Specific Columns**
```python
cursor.execute("SELECT name, email FROM users")
result = cursor.fetchall()
for row in result:
    print(row)
```

## 9. **Using WHERE Clause**
```python
cursor.execute("SELECT * FROM users WHERE name = 'John Doe'")
result = cursor.fetchall()
print(result)
```

## 10. **Using ORDER BY**
```python
cursor.execute("SELECT * FROM users ORDER BY name ASC")
result = cursor.fetchall()
print(result)
```

## 11. **Updating Records**
```python
sql = "UPDATE users SET email = %s WHERE name = %s"
values = ("newemail@example.com", "John Doe")
cursor.execute(sql, values)
conn.commit()
print(cursor.rowcount, "record updated.")
```

## 12. **Deleting Records**
```python
sql = "DELETE FROM users WHERE name = %s"
values = ("John Doe",)
cursor.execute(sql, values)
conn.commit()
print(cursor.rowcount, "record deleted.")
```

## 13. **Dropping a Table**
```python
cursor.execute("DROP TABLE users")
```

## 14. **Dropping a Database**
```python
cursor.execute("DROP DATABASE mydatabase")
```

## 15. **Using Prepared Statements to Prevent SQL Injection**
```python
sql = "SELECT * FROM users WHERE name = %s"
value = ("John Doe",)
cursor.execute(sql, value)
result = cursor.fetchall()
print(result)
```

## 16. **Closing Connection**
```python
cursor.close()
conn.close()
```

---
This markdown file covers all essential MySQL methods using Python. 🚀
