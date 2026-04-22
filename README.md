# 🧮 Postfix Expression Evaluator in C

A simple stack-based **postfix (Reverse Polish Notation) expression evaluator** written in C. It reads a postfix expression from the user and computes the result using a custom stack implementation.

---

## 📌 What is Postfix Notation?

In **postfix notation**, operators come *after* their operands — no parentheses needed!

| Infix Expression | Postfix Equivalent |
|------------------|--------------------|
| `2 + 3`          | `23+`              |
| `(2 + 3) * 5`    | `23+5*`            |
| `10 - 2 * 3`     | `1023*-`           |

---

## 🚀 Features

- Evaluates postfix expressions using a stack
- Supports four basic arithmetic operations: `+`, `-`, `*`, `/`
- Handles single-digit operands (0–9)
- Lightweight — no external libraries required

---

## 🛠️ How It Works

1. Scan each character of the expression left to right
2. If it's a **digit** → push it onto the stack
3. If it's an **operator** → pop two values, apply the operator, push the result
4. After scanning, the final result is on top of the stack

---

## 🖥️ Getting Started

### Prerequisites
- GCC compiler (or any C compiler)
- Linux / macOS / Windows (with MinGW or WSL)

### Compile & Run

```bash
gcc postfix.c -o postfix
./postfix
```

### Example

```
Enter postfix expression (e.g., 23+5*): 23+5*
Result = 25
```

**Explanation:** `(2 + 3) * 5 = 25`

---

## 📁 Project Structure

```
postfix-evaluator/
│
├── postfix.c      # Main source file
└── README.md      # Project documentation
```

---

## ⚙️ Code Overview

| Component     | Description                              |
|---------------|------------------------------------------|
| `stack[]`     | Integer array used as the stack          |
| `push(x)`     | Pushes an integer onto the stack         |
| `pop()`       | Pops and returns the top of the stack    |
| `main()`      | Reads input and evaluates the expression |

---

## ⚠️ Limitations

- Only supports **single-digit** operands (e.g., `0`–`9`)
- No error handling for invalid expressions or stack overflow
- Division by zero is not handled

---

## 🔮 Possible Improvements

- [ ] Support multi-digit numbers
- [ ] Add error handling for invalid input
- [ ] Extend to support `%` (modulus) and `^` (power)
- [ ] Add an infix-to-postfix converter

---

## 👨‍💻 Author

Made with ❤️ in C  
Feel free to fork, star ⭐, and contribute!

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
