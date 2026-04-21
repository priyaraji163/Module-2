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
def pascal_triangle(n):
    for i in range(n):
        row=[1]
        for j in range(1,i):
            row.append(prev_row[j-1]+prev_row[j])
        if i>0:
            row.append(1)
        print(" ".join(map(str,row)))
        prev_row=row
n=int(input())
pascal_triangle(n)
```


## Sample Output
<img width="452" height="406" alt="image" src="https://github.com/user-attachments/assets/0212cd67-1bfc-4c6d-8c05-849a2836ab6c" />


## Result
Thus,the Python program that generates Pascal's Triangle using numbers. The number of rows is accepted from the user is created successfully.

