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
~~~
def pascal_triangle(n):
    for i in range(n):
        print(" " * (n - i), end="")

        val = 1
        for j in range(i + 1):
            print(val, end=" ")
            val = val * (i - j) // (j + 1)
        print()

rows = int(input("Enter number of rows: "))
pascal_triangle(rows)
~~~


## Sample Output
<img width="650" height="248" alt="image" src="https://github.com/user-attachments/assets/48c4bb47-46ea-4a83-b38c-1b91b8614ee3" />

## Result
Thus,the program has been executed successfully.
