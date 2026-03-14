# 📁 03 — Data Structures
Learn how Python stores and organizes collections of data using Lists, Tuples, Sets, and Dictionaries.

---

## 📚 Topics Covered

### 📋 List (`lists.ipynb`)

| # | Topic | Description |
|---|---|---|
| 1 | Creating a List | Store multiple values in a single variable |
| 2 | Indexing | Access elements using index number |
| 3 | `append()` | Add one element to the end |
| 4 | `insert()` | Add element at a specific index |
| 5 | `remove()` | Remove first occurrence of a value |
| 6 | `extend()` | Add multiple elements to the end |
| 7 | `pop()` | Remove and return element by index |
| 8 | `reverse()` | Reverse the list in place |
| 9 | `sort()` | Sort elements ascending or descending |
| 10 | `len()` | Count total elements |
| 11 | `index()` | Find position of a value |
| 12 | `count()` | Count how many times a value appears |
| 13 | `copy()` | Make a duplicate list |
| 14 | `clear()` | Remove all elements |
| 15 | Slicing | Get a portion of a list |

### 🔒 Tuple (`tuples.ipynb`)

| # | Topic | Description |
|---|---|---|
| 1 | Creating a Tuple | Ordered, immutable collection |
| 2 | Indexing | Access elements using index number |
| 3 | `len()` | Count total elements |
| 4 | `index()` | Find position of a value |
| 5 | `count()` | Count occurrences of a value |
| 6 | Slicing | Get a portion of a tuple |
| 7 | Loop through Tuple | Iterate using for loop |
| 8 | Updating Tuple | Convert to list → update → convert back |

### 🔵 Set (`sets.ipynb`)

| # | Topic | Description |
|---|---|---|
| 1 | Creating a Set | Unordered collection of unique items |
| 2 | `add()` | Add a single element |
| 3 | `update()` | Add multiple elements |
| 4 | `remove()` | Remove element — error if not found |
| 5 | `discard()` | Remove element — no error if missing |
| 6 | `pop()` | Remove a random element |
| 7 | `len()` | Count elements |
| 8 | `clear()` | Remove all elements |
| 9 | `union()` | All elements from both sets |
| 10 | `intersection()` | Common elements only |
| 11 | `difference()` | Elements in first set but not second |

### 📖 Dictionary (`dictionaries.ipynb`)

| # | Topic | Description |
|---|---|---|
| 1 | Creating a Dictionary | Store data as key-value pairs |
| 2 | Accessing Values | Using `[ ]` and `get()` |
| 3 | Looping | Loop through keys, values, items |
| 4 | `keys()` | Return all keys |
| 5 | `values()` | Return all values |
| 6 | `items()` | Return all key-value pairs |
| 7 | `update()` | Add or update key-value pairs |
| 8 | `pop()` | Remove specific key, return value |
| 9 | `popitem()` | Remove last inserted pair |
| 10 | `setdefault()` | Add key only if it does not exist |
| 11 | `copy()` | Make a duplicate dictionary |
| 12 | `clear()` | Remove all items |
| 13 | `len()` | Count total key-value pairs |
| 14 | Nested Dictionary | Dictionary inside a dictionary |
| 15 | Quiz App Project | Terminal quiz using list of dictionaries |

---

## 📄 Files in This Folder

| File | Description |
|---|---|
| `lists.ipynb` | List creation, all methods, slicing, marks calculator project |
| `tuples.ipynb` | Tuple creation, methods, slicing, weekday loop project |
| `sets.ipynb` | Set creation, all methods, union/intersection/difference |
| `dictionaries.ipynb` | Dictionary methods, nested dict, Quiz App project |

---

## 💡 Key Concepts at a Glance
```python
# ── List ──────────────────────────────────────
fruits = ["Apple", "Banana", "Mango", "Orange"]
fruits.append("Kiwi")           # add to end
fruits.insert(1, "Cherry")      # add at index 1
fruits.remove("Banana")         # remove by value
fruits.pop()                    # remove last element
fruits.sort()                   # sort ascending
print(fruits[1:4])              # slicing


# ── Tuple ─────────────────────────────────────
marks = (50, 20, 40, 40, 80)
print(marks[0])                 # access by index
print(marks[1:4])               # slicing
print(marks.count(40))          # count occurrences

# Update workaround (tuples are immutable)
marks = list(marks)             # convert to list
marks[1] = 70                   # modify
marks = tuple(marks)            # convert back


# ── Set ───────────────────────────────────────
fruits = {"Apple", "Banana", "Mango"}
fruits.add("Orange")            # add one element
fruits.discard("Banana")        # remove safely

set1 = {1, 2, 3}
set2 = {3, 4, 5}
print(set1.union(set2))         # {1, 2, 3, 4, 5}
print(set1.intersection(set2))  # {3}
print(set1.difference(set2))    # {1, 2}


# ── Dictionary ────────────────────────────────
student = {
    "name"    : "Ali Hassan",
    "age"     : 17,
    "gpa"     : 3.8,
    "active"  : True,
    "subjects": ["Math", "CS"]
}
print(student["name"])              # bracket access
print(student.get("phone", "N/A")) # safe access
student.update({"city": "Lahore"}) # add new key
student.pop("age")                  # remove key

for key, value in student.items():  # loop
    print(key, ":", value)
```

---

## 🆚 Quick Comparison Table

| Feature | List | Tuple | Set | Dictionary |
|---|---|---|---|---|
| Syntax | `[ ]` | `( )` | `{ }` | `{ key: val }` |
| Ordered | ✅ Yes | ✅ Yes | ❌ No | ✅ Yes (3.7+) |
| Mutable | ✅ Yes | ❌ No | ✅ Yes | ✅ Yes |
| Duplicates | ✅ Allowed | ✅ Allowed | ❌ No | ❌ No duplicate keys |
| Indexed | By position | By position | ❌ No index | By key |
| Use case | Ordered items | Fixed data | Unique values | Key-value data |

---

## ✅ Practice Tasks
```python
# Task 1 — List
# Create a list of 5 student names
# Add a new name using append()
# Remove the 3rd student using pop()
# Sort the list alphabetically and print it

# Task 2 — Tuple
# Create a tuple of 5 subject names
# Print the first and last subject using indexing
# Count how many times "Math" appears

# Task 3 — Set
# Create two sets of student roll numbers
# Print students present in BOTH sets (intersection)
# Print students present in either set (union)

# Task 4 — Dictionary
# Create a dictionary for a student with keys:
# name, age, grade, city
# Print all keys and all values separately
# Update the grade and add a new key "phone"
# Delete the "city" key and print the final dictionary

# Task 5 — Quiz App (Project)
# Build a 5-question quiz using a list of dictionaries
# Each dictionary must have: question, options, answer
# Show score, percentage, and Pass/Fail at the end
```

---

## 🎯 Who Is This For?

- ✅ Grade 10–12 students (FBISE / Cambridge IGCSE)
- ✅ BS Computer Science — Semester 1 students
- ✅ Anyone who completed 02 — Control Flow
- ✅ Self-learners preparing for programming interviews

---

## ▶️ How To Run

**Option 1 — View online:** Click any `.ipynb` file directly on GitHub to read notes and outputs.

**Option 2 — Run locally:**
```bash
git clone https://github.com/umaraihub/Python-Programming.git
cd Python-Programming/03_Data_Structures
jupyter notebook
```

---

## 🔗 Navigation

| Previous | Current | Next |
|---|---|---|
| 📂 02 Control Flow ← | 📂 03 Data Structures | 📂 04 Functions → |

Part of the 🐍 **Python Programming** repository by **Muhammad Umar**
