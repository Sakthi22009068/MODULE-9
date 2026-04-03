# # ➖ Matrix Operations-Matrix Subtraction in Python

## 🎯 AIM:
To write a Python program that reads two matrices from the user and performs matrix subtraction.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` for rows and columns
3. Get the values of `r` and `c` from the user
4. Define a function `create_matrix(n, m)` to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the `create_matrix()` function twice to read two matrices `A` and `B`
6. Define a loop to subtract the elements of matrix `B` from matrix `A`
7. Store the result in a new matrix `C`
8. Print the resulting matrix `C`
9. **Stop**

---

## 💻 PROGRAM:

def create_matrix(r, c):

    matrix = []
    
    print("Enter matrix elements row-wise:")
    
    for i in range(r):
    
        row = list(map(int, input().split()))
        
        matrix.append(row)
        
    return matrix

r = int(input("Enter number of rows: "))

c = int(input("Enter number of columns: "))

print("\nEnter Matrix A:")

A = create_matrix(r, c)

print("\nEnter Matrix B:")

B = create_matrix(r, c)

C = []

for i in range(r):

    row = []
    
    for j in range(c):
    
        row.append(A[i][j] - B[i][j])
        
    C.append(row)


print("\nResultant Matrix (A - B):")

for row in C:

    print(row)


## OUTPUT:
Enter number of rows: 2

Enter number of columns: 2

Enter Matrix A:
1 2
3 4

Enter Matrix B:
4 3
2 1

Resultant Matrix (A - B):
[-3, -1]
[1, 3]
## RESULT:
The program successfully performs matrix subtraction (A − B) by subtracting corresponding elements of two matrices and storing the result in a new matrix.

