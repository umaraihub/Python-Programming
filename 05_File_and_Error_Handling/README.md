# 📁 05 — File & Error Handling
Learn how to read, write, and manage files in Python,
and how to handle errors gracefully using try/except.

---

## 📚 Topics Covered

### 📁 File Handling (`file_handling.ipynb`)

| # | Topic | Description |
|---|---|---|
| 1 | `open()` | Open a file with different modes |
| 2 | File Modes | r, w, a, x, r+, w+, a+ |
| 3 | `write()` | Write a single string to file |
| 4 | `writelines()` | Write multiple lines at once |
| 5 | `read()` | Read entire file content |
| 6 | `readline()` | Read one line at a time |
| 7 | `readlines()` | Read all lines as a list |
| 8 | `append` | Add content without overwriting |
| 9 | `seek()` & `tell()` | File pointer position |
| 10 | `os.remove()` | Delete a file |
| 11 | `os.rename()` | Rename a file |
| 12 | `os.path.exists()` | Check if file exists |
| 13 | `with` statement | Auto close file safely |

### ⚠️ Error Handling (`error_handling.ipynb`)

| # | Topic | Description |
|---|---|---|
| 1 | `try` / `except` | Handle errors without crashing |
| 2 | `Exception` | Catch all common errors |
| 3 | `Exception as e` | Print actual error message |
| 4 | `NameError` | Variable not defined error |
| 5 | `FileNotFoundError` | File does not exist error |
| 6 | `PermissionError` | No access to file error |
| 7 | `ZeroDivisionError` | Division by zero error |
| 8 | `ValueError` | Invalid value error |
| 9 | `else` block | Runs only if no error occurs |
| 10 | `finally` block | Always runs regardless of error |
| 11 | Project | Dynamic file mode selector |

---

## 📄 Files in This Folder

| File | Description |
|---|---|
| `file_handling.ipynb` | File modes, read, write, append, seek, os module |
| `error_handling.ipynb` | try/except, multiple errors, else, finally, project |

---

## 💡 Key Concepts at a Glance
```python
# ── Write to File ─────────────────────────────
with open("data.txt", "w") as file:
    file.write("Name: Umar Jee\n")
    file.write("Age: 26\n")
    file.write("City: Islamabad\nAddress: Near Rawalpindi")

# ── Read from File ────────────────────────────
with open("data.txt", "r") as file:
    content = file.read()
    print(content)

# ── Append to File ────────────────────────────
with open("data.txt", "a") as file:
    file.write("\nFavorite Subject: Python")

# ── Error Handling ────────────────────────────
try:
    with open("data.txt", "r") as file:
        content = file.read()
        print(content)
except FileNotFoundError:
    print("File Not Found")
except PermissionError:
    print("No permission to access file.")
except Exception as e:
    print("Unexpected Error:", e)
else:
    print("File operation completed successfully.")
finally:
    print("Program execution finished.")

# ── Check & Delete File ───────────────────────
import os
if os.path.exists("data.txt"):
    os.remove("data.txt")
    print("File deleted!")
else:
    print("File does not exist!")
```

---

## 🆚 File Modes Quick Reference

| Mode | Creates | Reads | Writes | Overwrites |
|---|---|---|---|---|
| `r` | ❌ | ✅ | ❌ | ❌ |
| `w` | ✅ | ❌ | ✅ | ✅ |
| `a` | ✅ | ❌ | ✅ | ❌ |
| `x` | ✅ | ❌ | ✅ | ❌ |
| `r+` | ❌ | ✅ | ✅ | ❌ |
| `w+` | ✅ | ✅ | ✅ | ✅ |
| `a+` | ✅ | ✅ | ✅ | ❌ |

---

## 🔗 Navigation

| Previous | Current | Next |
|----------|---------|------|
| [📂 04 Functions ←](../04_Functions/) | 📂 05 File & Error Handling | [📂 06 OOP →](../06_OOP/) |

---

*Part of the [🐍 Python Programming](../README.md) repository by **Muhammad Umar***
