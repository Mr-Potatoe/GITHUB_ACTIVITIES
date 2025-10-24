## 🧩 **GROUP 1 – Smart Temperature & Weather Alert**

**Goal:** Convert temperature, display weather category, and store multiple records.
**Concepts:** Variables, Lists, Loops, If-Else, Functions

**New Features:**

* Accept multiple temperature inputs (loop until user types “stop”).
* Store conversions in a **list of dictionaries**.
* Function `convert_temp(value, unit)` handles both conversions.
* Function `analyze_weather(celsius)` categorizes conditions.
* At the end, display an average temperature summary.

**Sample Flow:**

```python
# Output Example
Enter temp (C/F or 'stop'): 30C
30°C = 86°F | Pleasant Day
Enter temp (C/F or 'stop'): 100F
100°F = 37.78°C | Hot Day
Enter temp (C/F or 'stop'): stop

Average: 33.89°C | Overall: Warm Climate
```

---

## 🧮 **GROUP 2 – Student Grading & Performance Analyzer**

**Goal:** Manage multiple students, compute GPA, and assign class honors.
**Concepts:** Lists, Dictionaries, Loops, Functions, Decisions

**New Features:**

* Loop for multiple students; stop when “exit” is typed.
* Store each student’s name, grades, GPA, and remark in a **dictionary**.
* Function `compute_gpa(grades)` and `remark(gpa)` handle logic.
* End report shows class average and top performer.

**Sample Flow:**

```python
Student Name: Aria
Enter 5 grades: 90 85 88 92 91
GPA: 89.2 | Remark: Satisfactory

Student Name: Leo
Enter 5 grades: 95 94 96 93 97
GPA: 95.0 | Remark: Outstanding

Class Average: 92.1 | Top Student: Leo
```

---

## 💰 **GROUP 3 – ATM System with Security, Transaction Logs & Receipt**

**Goal:** Build a secure ATM simulation with login, balance tracking, and receipts.
**Concepts:** While Loops, If-Else, Functions, Lists, Strings

**New Features:**

* PIN login with lockout after 3 failed attempts.
* Separate functions: `deposit()`, `withdraw()`, `check_balance()`, `print_receipt()`.
* Maintain a **transaction log list** recording each operation.
* Add option to show all transactions before exit.
* Print a mini “receipt” at the end with totals.

**Sample Flow:**

```
Enter PIN: 1234
1. Deposit  2. Withdraw  3. Balance  4. Transactions  5. Exit
Deposit ₱500 → New Balance: ₱1500
Withdraw ₱200 → New Balance: ₱1300
--- Session Summary ---
Deposited: ₱500 | Withdrawn: ₱200 | Final Balance: ₱1300
Transactions:
[Deposit: ₱500, Withdraw: ₱200]
```

---

## ⚕️ **GROUP 4 – BMI & Health Recommendation System**

**Goal:** Compute BMI for multiple users, classify health, and provide recommendations.
**Concepts:** Functions, Lists, If-Else, Loops, String Formatting

**New Features:**

* Function `bmi(weight, height)` and `recommendation(status)` for advice.
* Loop for multiple users (family health tracker).
* Store results in a **list of dictionaries** with names, BMI, and status.
* Add logic for ideal weight range based on height.
* Display overall health summary (how many are normal/overweight/etc.).

**Sample Flow:**

```
Name: Sarah | BMI: 23.5 | Status: Normal | Advice: Keep balanced meals.
Name: Kai | BMI: 29.2 | Status: Overweight | Advice: Regular exercise needed.
Summary: 1 Normal, 1 Overweight
```

---

## 🛒 **GROUP 5 – E-Commerce Cart & Discount System**

**Goal:** Create a smart shopping cart with categories, discounts, and inventory check.
**Concepts:** Lists, Dictionaries, Loops, Functions, Math Operators

**New Features:**

* Menu with product categories (Electronics, Clothes, Food).
* Each category has **items and stock quantities** (use dictionary).
* Function `add_to_cart(item, qty)` checks stock and updates it.
* Function `checkout()` applies discount tiers:

  * ≥₱2000 → 25%
  * ≥₱1000 → 15%
  * ≥₱500 → 10%
* Show receipt: item list, subtotal, discount, total, and savings.

**Sample Flow:**

```
Available: {Phone: 800, Shirt: 300, Bread: 100}
Added: Phone x2, Shirt x1
Subtotal: ₱1900 | Discount: 15% | Total: ₱1615
Remaining Stock: {Phone: 0, Shirt: 4, Bread: 10}
```

---

## 🧾 **GROUP 6 – Library Book Borrowing & Return System**

**Goal:** Create a simple library system that manages books, borrowers, and due dates.
**Concepts:** Variables, Lists, Dictionaries, Control Structures, Functions, Loops

**Features:**

* Store available books in a **dictionary** with copies left.
* Function `borrow_book(name, title)` checks if the book exists and is available.
* Function `return_book(name, title)` adds the copy back and calculates any **late fee**.
* Record transactions in a **list of dictionaries** with borrower name, book title, and status.
* Apply a **fine** of ₱10 per day if overdue (simulate with user input).
* Add menu options: View Books, Borrow, Return, View Records, Exit.

---

**Instructions:**

1. Display available books with copies.
2. Use a **while loop** to show options repeatedly.
3. On borrowing:

   * Check if stock > 0
   * If yes, decrease stock and log the transaction
4. On returning:

   * Ask how many days late (if any)
   * Compute fine = days * 10
   * Add the copy back to inventory
5. On exit, display a summary of all transactions and remaining books.

---

**Sample Flow:**

```
Available Books:
{"Python 101": 3, "AI Basics": 2, "Data Mining": 1}

1. Borrow Book
2. Return Book
3. View Records
4. Exit

Choice: 1
Name: Aria | Book: Python 101
Book borrowed successfully!

Choice: 2
Name: Aria | Book: Python 101 | Days Late: 2
Returned successfully. Fine: ₱20

--- Summary ---
Borrowed: Python 101 by Aria
Returned: Python 101 | Fine: ₱20
Remaining Books: {"Python 101": 3, "AI Basics": 2, "Data Mining": 1}
```

---
