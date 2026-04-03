# 🧮 SORTING ALGORITHMS: Insertion Sort Using a Class

This program demonstrates how to implement the **Insertion Sort algorithm** using a Python class. It allows the user to input a list of numbers, sorts them using the insertion sort technique, and displays the sorted list.

---

## 🎯 Aim

To develop a Python class with functions to:
- Create a list of integers
- Sort it using the **Insertion Sort** algorithm
- Display the sorted list

---

## 🧠 Algorithm

1. **Start the program**
2. **Define a class** `InsertionSorter`
3. Inside the class:
   - `create_list()`:
     - Read number of elements
     - Store them in a list
   - `insertion_sort()`:
     - Iterate from the second element to the end
     - Move elements greater than the key to one position ahead
     - Insert the key at the correct position
   - `print_list()`:
     - Print the sorted list
4. **Create an object** of the class
5. **Call** the methods in order: `create_list()`, `insertion_sort()`, and `print_list()`
6. **End the program**

---

## 💻 PROGRAM:

class InsertionSorter:
    
    def __init__(self):
    
        self.arr = []

    # Method to create list
    
    def create_list(self):
    
        n = int(input("Enter number of elements: "))
        
        print("Enter elements:")
        
        self.arr = list(map(int, input().split()))
    
    # Method to perform insertion sort
    
    def insertion_sort(self):
    
        for i in range(1, len(self.arr)):
        
            key = self.arr[i]
            
            j = i - 1
            
            # Move elements greater than key one position ahead
            
            while j >= 0 and self.arr[j] > key:
            
                self.arr[j + 1] = self.arr[j]
                
                j -= 1
            
            self.arr[j + 1] = key

    # Method to print list
    
    def print_list(self):
    
        print("Sorted list:", self.arr)

obj = InsertionSorter()

obj.create_list()

obj.insertion_sort()

obj.print_list()



## OUTPUT:
Enter number of elements: 5

Enter elements:

5 2 9 1 6

Sorted list: [1, 2, 5, 6, 9]

## RESULT:
The program successfully implements the Insertion Sort algorithm using a class, allowing the user to input elements, sort them step-by-step, and display the sorted list.
