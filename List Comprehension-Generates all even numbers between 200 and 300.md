# 🧾 List Comprehension:Generates all even numbers between 200 and 300
## 🎯 AIM:
To write a Python class-based program that generates all even numbers between 200 and 300 using **list comprehension**, and stores them in a list.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create a class named `program`
3. Create variables `a`, `b`, and `c` to represent:
   - `a`: Lower limit
   - `b`: Step value
   - `c`: Upper limit
4. Initialize the values using a constructor `__init__`
5. Define a method `display()` that uses **list comprehension** to store even numbers
6. Print the resulting list of even numbers
7. **Stop**

---

## 💻 PROGRAM:


class program:

    def __init__(self, a, b, c):
    
        self.a = a  # lower limit
        
        self.b = b  # step value
        
        self.c = c  # upper limit

    def display(self):
    
        # List comprehension to generate even numbers
        
        even_numbers = [i for i in range(self.a, self.c + 1, self.b) if i % 2 == 0]
        
        print("Even numbers between", self.a, "and", self.c, "are:")'
        
        print(even_numbers)

obj = program(200, 1, 300)


obj.display()


## OUTPUT:
Even numbers between 200 and 300 are:

[200, 202, 204, 206, 208, 210, 212, 214, 216, 218, 220, 222, 224, 226, 228, 230, 232, 234, 236, 238, 240, 242, 244, 246, 248, 250, 252, 254, 256, 258, 260, 262, 264, 266, 268, 270, 272, 274, 276, 278, 280, 282, 284, 286, 288, 290, 292, 294, 296, 298, 300]

## RESULT:
The program successfully uses list comprehension inside a class method to generate and display all even numbers between 200 and 300, demonstrating efficient and concise Python programming.
