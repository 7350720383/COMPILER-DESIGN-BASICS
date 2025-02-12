### **Simple Arithmetic Expression Compiler**

This C++ program is a simple arithmetic expression parser and evaluator. It can take a mathematical expression as input, parse it using a recursive descent approach, and compute the result while following standard operator precedence rules.

---

## **Features**
✅ Supports basic arithmetic operations:  
   - Addition (`+`), Subtraction (`-`), Multiplication (`*`), and Division (`/`).

✅ Handles **operator precedence**:  
   - Multiplication and division have higher precedence than addition and subtraction.  
   - Parentheses `()` allow users to explicitly define operation order.

✅ Supports **floating-point numbers**.

✅ Ignores whitespace in the input.

---

## **How It Works**
The program uses **recursive descent parsing**, breaking down expressions into different levels:

1. **Lexical Analysis (Tokenizer)**
   - Reads characters one by one, ignoring whitespace.
   - Identifies numbers, operators, and parentheses.

2. **Parsing (Recursive Descent)**
   - **`factor()`**: Handles numbers and parentheses.
   - **`term()`**: Handles multiplication (`*`) and division (`/`).
   - **`expression()`**: Handles addition (`+`) and subtraction (`-`).

3. **Evaluation**
   - The parser computes results by following operator precedence.

---

## **Example Inputs and Outputs**
### **Input 1**:
```
Enter an arithmetic expression: (3 + 5) * 2
```
### **Output 1**:
```
Result: 16
```
---

### **Input 2**:
```
Enter an arithmetic expression: 10 + 2 * 3
```
### **Output 2**:
```
Result: 16
```
*(Multiplication is evaluated first, then addition.)*

---

### **Input 3**:
```
Enter an arithmetic expression: (10 + 2) / 4
```
### **Output 3**:
```
Result: 3
```
*(Parentheses force `10 + 2` to be evaluated first.)*

---

## **Enhancements & Future Improvements**
🔹 Handle invalid inputs (e.g., `5 ++ 3` or `10 / 0`).  
🔹 Support for exponentiation (`^`).  
🔹 Adding variable storage and assignment support.  
🔹 More complex mathematical functions (e.g., `sin()`, `cos()`, `sqrt()`).  
