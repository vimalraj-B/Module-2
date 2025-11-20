# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.


## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

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


## 🧪 Program
## Developed By : VIMALRAJ B
## Register Number : 212224230304
```
def print_pascal_triangle(size):
    for i in range(0,size):
        for j in range(0,i+1):
            print(decide_number(i,j),end=" ")
        print()
def decide_number(n,k):
    num=1
    if k>n-k:
        k=n-k
    for i in range(0,k):
        num=num*(n-i)
        num=num//(i+1)
    return num
rows=int(input())
print_pascal_triangle(rows)
```
## Sample Output

<img width="667" height="711" alt="image" src="https://github.com/user-attachments/assets/d28ef494-4dd6-4511-a2aa-2b92bede5a64" />


## Result

Thus , the program executed Successfully.
