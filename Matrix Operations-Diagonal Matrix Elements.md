# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## 📌 Aim

To write a Python program that prints only the diagonal elements of a given matrix.

## 🧠 Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

## 🖥️ Program

rows = int(input("Enter number of rows: "))

cols = int(input("Enter number of columns: "))

matrix = []

print("Enter matrix elements row-wise:")

for i in range(rows):

    row = list(map(int, input().split()))
    
    matrix.append(row)


print("\nOriginal Matrix:")

for row in matrix:

    print(row)


print("\nDiagonal Matrix:")

for i in range(rows):

    for j in range(cols):
    
        if i == j:
        
            print(matrix[i][j], end=" ")
            
        else:
        
            print(" ", end=" ")
            
    print()

### Output:
Enter number of rows: 3
Enter number of columns: 3
Enter matrix elements row-wise:
1 2 3
4 5 6
7 8 9

Original Matrix:
[1, 2, 3]
[4, 5, 6]
[7, 8, 9]

Diagonal Matrix:
1     
 5    
   9

## Result
The program successfully reads a matrix and prints only the main diagonal elements, leaving other positions blank, demonstrating correct matrix traversal and conditional logic.
