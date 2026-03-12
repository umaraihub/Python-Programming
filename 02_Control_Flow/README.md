
# 📁 02 — Control Flow

> Learn how Python makes decisions and repeats actions using conditions and loops.

---

## 📚 Topics Covered

### 🔀 Conditional Statements (`conditions.ipynb`)

| # | Topic | Description |
|---|-------|-------------|
| 1 | if Statement | Executes a block only when condition is True |
| 2 | if / else Statement | Executes if block when True, else block when False |
| 3 | if / elif / else | Handles more than two conditions in sequence |
| 4 | Nested if | An if statement inside another if statement |

### 🔁 Loops & Loop Control (`loops.ipynb`)

| # | Topic | Description |
|---|-------|-------------|
| 5 | for Loop | Repeats code over a sequence or range |
| 6 | while Loop | Repeats code while condition remains True |
| 7 | break Statement | Exits the loop immediately |
| 8 | continue Statement | Skips current iteration and moves to next |
| 9 | pass Statement | Placeholder for an empty block |

---

## 📄 Files in This Folder

| File | Description |
|------|-------------|
| `conditions.ipynb` | if, if/else, if/elif/else, Nested if — with real examples |
| `loops.ipynb` | for loop, while loop, break, continue, pass — with real examples |

---

## 💡 Key Concepts at a Glance
```python
# ── if Statement ──────────────────────────────
marks = int(input("Enter Your Marks = "))
if marks > 40:
    print("PASS")           # runs only if condition is True


# ── if / else Statement ───────────────────────
age = int(input("Enter Your Age = "))
if age >= 18:
    print("Eligible for Driving License.")
else:
    print("Not Eligible for Driving License.")


# ── if / elif / else ──────────────────────────
num = int(input("Enter a Number = "))
if num > 0:
    print("Positive Number")
elif num < 0:
    print("Negative Number")
else:
    print("Equal to Zero")


# ── Nested if ─────────────────────────────────
username = "umar"
password = "umar1234"
if username == "umar":
    if password == "umar1234":
        print("Login Successful")
    else:
        print("Wrong Password")
else:
    print("Username Not Found")
```

---

## 🔄 if vs if/else vs if/elif/else

| Statement | Use When | Outcomes |
|---|---|---|
| `if` | Only one condition to check | 1 possible outcome |
| `if / else` | Two possible outcomes | Always 1 of 2 runs |
| `if / elif / else` | More than two conditions | Always 1 of many runs |
| `Nested if` | Second condition depends on first | Multiple level checking |

---

## ✅ Practice Tasks
```python
# Task 1 — if Statement
# Ask user to enter temperature
# If temperature is greater than 40, print "Very Hot"

# Task 2 — if / else Statement
# Ask user to enter a number
# Print whether the number is Even or Odd

# Task 3 — if / elif / else
# Ask user to enter marks (0–100)
# Print grade: 90+=A+, 80+=A, 70+=B, 60+=C, 50+=D, below 50=F

# Task 4 — Nested if
# Ask user to enter a number
# Check if Positive or Negative
# If Positive — also check if Even or Odd
```

---

## 🎯 Who Is This For?

- ✅ Grade 10–12 students (FBISE / Cambridge IGCSE)
- ✅ BS Computer Science — Semester 1 students
- ✅ Anyone who completed 01 — Python Fundamentals
- ✅ Self-learners preparing for programming interviews

---

## ▶️ How To Run

**Option 1 — View online:**
Click any `.ipynb` file directly on GitHub to read notes and outputs.

**Option 2 — Run locally:**
```bash
git clone https://github.com/umaraihub/Python-Programming.git
cd Python-Programming/02_Control_Flow
jupyter notebook
```

---

## 🔗 Navigation

| Previous | Current | Next |
|----------|---------|------|
| [📂 01 Fundamentals ←](../01_Fundamentals/) | 📂 02 Control Flow | [📂 03 Data Structures →](../03_Data_Structures/) |

---

*Part of the [🐍 Python Programming](../README.md) repository by **Muhammad Umar***
