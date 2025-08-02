
## ✅ **Project Title:**

**Scientific Calculator in C++**

---

## 📌 **Objective:**

To develop a console-based **scientific calculator** using C++ that can perform basic arithmetic as well as advanced mathematical operations such as trigonometric, logarithmic, exponential, and factorial calculations.

---

## 🛠️ **Tools and Technologies Used:**

* **Language:** C++
* **Compiler:** g++, Turbo C++, or any standard C++ compiler
* **Libraries Used:**

  * `<iostream>` – for input/output operations
  * `<cmath>` – for mathematical functions like `sin()`, `cos()`, `log()`, `sqrt()`, etc.

---

## 🧠 **Working Principle & Logic:**

### 🧮 1. **User Interface (Text Menu)**

* The program starts by displaying a **menu of options**.
* The user selects an operation by entering the corresponding number (1 to 12 or 0 to exit).
* The menu is presented inside a loop (`do...while`) so that the user can perform multiple operations without restarting the program.

---

### 🔢 2. **Basic Operations**

These operations use simple arithmetic:

```cpp
result = num1 + num2;
result = num1 - num2;
result = num1 * num2;
result = num1 / num2;
```

* Input: Two numbers from the user.
* Output: Result printed directly.
* **Division** includes a check to prevent division by zero.

---

### 🧮 3. **Power and Square Root**

* `pow(x, y)` calculates $x^y$
* `sqrt(x)` returns square root. A check ensures input is non-negative.

---

### 📉 4. **Logarithmic Functions**

* `log10(x)` gives base-10 logarithm.
* `log(x)` gives natural log (ln base *e*).
* Input must be **positive**, else the function returns NaN or runtime error.

---

### 📐 5. **Trigonometric Functions (in degrees)**

* `sin`, `cos`, and `tan` functions use radians, so the degree input is **converted to radians**:

  $$
  \text{radians} = \text{degrees} \times \left(\frac{\pi}{180}\right)
  $$
* Used constant `M_PI` from `<cmath>` to represent π.

---

### ➗ 6. **Factorial**

```cpp
long long factorial(int n) {
    if (n < 0) return -1; // Invalid
    long long fact = 1;
    for (int i = 2; i <= n; ++i)
        fact *= i;
    return fact;
}
```

* Accepts only **non-negative integers**.
* Calculated using a loop (iterative method).
* Long long type is used to handle large results.
* Input is checked to be whole (not decimal) before proceeding.

---

### 🔁 7. **Control Flow**

* `do...while` loop allows repeated use until user chooses `0` to exit.
* `switch...case` is used for selecting operation based on user's input.
* `cin.fail()` is checked to handle any wrong input types (e.g., entering a letter instead of a number).

---

### ⚠️ 8. **Error Handling**

* Each sensitive operation checks for invalid conditions:

  * Division by zero
  * Log of zero or negative numbers
  * Square root of negative numbers
  * Factorial of negative or non-integer values

---

## 📋 **Sample Output:**

```
===== Scientific Calculator =====

Choose an operation:
1. Addition
2. Subtraction
...
12. Factorial
0. Exit
Enter your choice: 5
Enter base and exponent: 2 3
Result: 8
```

---

## ✅ **Advantages of the Project:**

* Demonstrates **core C++ skills**: I/O, loops, conditional logic, functions.
* Uses **standard math library** effectively.
* Provides **user-friendly interface** and **error-handling**.
* Can be easily **extended** with GUI, complex numbers, or history feature.

---

## 📚 **Learning Outcomes:**

* Use of standard C++ math functions.
* Structuring programs using functions and control statements.
* Implementing menus and user choices.
* Basic understanding of input validation and error handling.
