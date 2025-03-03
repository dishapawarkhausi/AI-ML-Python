# Python File Handling - All Important Commands

## 1. **Opening and Closing Files**
```python
file = open("example.txt", "r")  # Open a file in read mode
file.close()  # Close the file
```

| Mode | Description |
|------|------------|
| `"r"` | Read mode (default) |
| `"w"` | Write mode (overwrites existing file) |
| `"a"` | Append mode (adds content at the end) |
| `"x"` | Create mode (fails if file exists) |
| `"b"` | Binary mode (e.g., images) |
| `"t"` | Text mode (default) |

## 2. **Reading Files**
```python
with open("example.txt", "r") as file:
    content = file.read()  # Read entire file
    print(content)
```

- **Read a specific number of characters:**
  ```python
  file.read(10)  # Reads first 10 characters
  ```
- **Read line by line:**
  ```python
  file.readline()  # Reads one line
  file.readlines()  # Reads all lines into a list
  ```

## 3. **Writing Files**
```python
with open("example.txt", "w") as file:
    file.write("Hello, World!\n")  # Overwrites file with text
```

- **Appending to a file:**
  ```python
  with open("example.txt", "a") as file:
      file.write("Appending new content!\n")
  ```

## 4. **Working with Binary Files**
```python
with open("image.jpg", "rb") as file:
    binary_data = file.read()
```
```python
with open("copy.jpg", "wb") as file:
    file.write(binary_data)
```

## 5. **Checking if a File Exists**
```python
import os
if os.path.exists("example.txt"):
    print("File exists")
else:
    print("File not found")
```

## 6. **Deleting Files**
```python
import os
os.remove("example.txt")  # Deletes the file
```

## 7. **Renaming and Moving Files**
```python
import os
os.rename("old_name.txt", "new_name.txt")
```

## 8. **Working with Directories**
```python
os.mkdir("new_folder")  # Create a new directory
os.rmdir("new_folder")  # Remove an empty directory
os.listdir(".")  # List files in current directory
```

## 9. **Using File Paths (Cross-Platform Support)**
```python
from pathlib import Path
file_path = Path("example.txt")
print(file_path.exists())  # Check if file exists
```

---
This guide covers all essential file handling commands in Python. 🚀
