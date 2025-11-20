# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
ef factorial(n):
 if n == 0 or n == 1:
 return 1
 return n * factorial(n - 1)
def combination(n, k):
 return factorial(n) // (factorial(k) * factorial(n - k))
# Step 2: Input from user
num_rows = int(input())
# Step 5: Generate Pascal's Triangle
for i in range(num_rows):
 # Step 5.1: Print spaces
 print(' ' * (num_rows - i - 1), end='')
 # Step 5.2: Print values in the row
for j in range(i + 1):
 print(combination(i, j), end=' ')

 # Step 5.3: Move to next line
 print()
```

## Sample Output
<img width="205" height="232" alt="image" src="https://github.com/user-attachments/assets/62274827-7a9d-4985-addf-19033f19cb89" />

## Result
Thus, the program has been successfully executed
