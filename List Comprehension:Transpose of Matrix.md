# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---

## 💻 PROGRAM:

def create(r, c):

    matrix = []
    
    print("Enter matrix elements row-wise:")
    
    for i in range(r):
    
        row = list(map(int, input().split()))
        
        matrix.append(row)
        
    return matrix


r = int(input("Enter number of rows: "))

c = int(input("Enter number of columns: "))

matrix = create(r, c)


transpose = [[matrix[i][j] for i in range(r)] for j in range(c)]

print("\nOriginal Matrix:")

for row in matrix:

    print(row)

print("\nTransposed Matrix:")

for row in transpose:

    print(row)
    


## OUTPUT:
Enter number of rows: 2

Enter number of columns: 3

Enter matrix elements row-wise:
1 2 3
4 5 6

Original Matrix:
[1, 2, 3]
[4, 5, 6]

Transposed Matrix:
[1, 4]
[2, 5]
[3, 6]

## RESULT:
The program successfully computes the transpose of a matrix using list comprehension, converting rows into columns efficiently.


