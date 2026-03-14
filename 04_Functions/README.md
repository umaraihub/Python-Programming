# 📁 04 — Functions
Learn how to write reusable blocks of code using Python functions.

---

## 📚 Topics Covered

### 🔧 Functions (`functions.ipynb`)

| # | Topic | Description |
|---|---|---|
| 1 | `def` | Define and call a reusable block of code |
| 2 | Positional Arguments | Arguments passed in order |
| 3 | Keyword Arguments | Arguments passed by key name |
| 4 | Default Arguments | Value used if argument not provided |
| 5 | `*args` | Accept multiple positional arguments as tuple |
| 6 | `**kwargs` | Accept multiple keyword arguments as dictionary |
| 7 | `return` | Send a value back from function to caller |

### 🔍 Scope (`scope.ipynb`)

| # | Topic | Description |
|---|---|---|
| 1 | Local Variable | Defined inside function — accessible only inside |
| 2 | Global Variable | Defined outside function — accessible everywhere |

### λ Lambda (`lambda.ipynb`)

| # | Topic | Description |
|---|---|---|
| 1 | Lambda Function | Small anonymous one-line function |
| 2 | `map()` | Apply function to every item in a list |
| 3 | `filter()` | Keep only items that match a condition |
| 4 | `sorted()` | Sort using custom lambda key |

### ⚙️ Built-in Functions (`builtin_functions.ipynb`)

| # | Topic | Description |
|---|---|---|
| 1 | `enumerate()` | Get index and value together while looping |
| 2 | `zip()` | Combine two or more lists together |
| 3 | `id()` | Get memory address of a variable |
| 4 | `help()` | Show documentation of any function |

---

## 📄 Files in This Folder

| File | Description |
|---|---|
| `functions.ipynb` | def, all argument types, return statement |
| `scope.ipynb` | Local and global variables |
| `lambda.ipynb` | Lambda functions with map, filter, sorted |
| `builtin_functions.ipynb` | enumerate, zip, id, help |

---

## 💡 Key Concepts at a Glance
```python
# ── def & return ──────────────────────────────
def add(a, b):
    return a + b

result = add(5, 3)
print(result)             # 8

# ── *args ─────────────────────────────────────
def student(name, *skills):
    print("Name :", name)
    for skill in skills:
        print("-", skill)

student("Arslan", "Python", "Gen AI", "Prompt Engineering")

# ── **kwargs ──────────────────────────────────
def student(**info):
    for key, value in info.items():
        print(key, ":", value)

student(name="Arslan", age=27, city="Islamabad")

# ── Scope ─────────────────────────────────────
name = "Muhammad Umar"    # global variable

def show():
    x = 10                # local variable
    print(name)           # global accessible inside
    print(x)              # local accessible inside

# ── Lambda ────────────────────────────────────
square  = lambda x    : x ** 2
add     = lambda a, b : a + b

numbers = [1, 2, 3, 4, 5]
squares = list(map(lambda n : n**2,       numbers))  # [1,4,9,16,25]
evens   = list(filter(lambda x : x%2==0, numbers))  # [2,4]

# ── Built-in Functions ────────────────────────
fruits = ["Apple", "Banana", "Mango"]

for index, fruit in enumerate(fruits, start=1):
    print(f"{index}. {fruit}")

names  = ["Ali",  "Sara",  "Ahmed"]
marks  = [85,      92,      78]
for name, mark in zip(names, marks):
    print(f"{name} : {mark}")
```

---

## 🔗 Navigation

| Previous | Current | Next |
|----------|---------|------|
| [📂 03 Data Structures ←](../03_Data_Structures/) | 📂 04 Functions | [📂 05 File & Error Handling →](../05_File_and_Error_Handling/) |

---

*Part of the [🐍 Python Programming](../README.md) repository by **Muhammad Umar***
