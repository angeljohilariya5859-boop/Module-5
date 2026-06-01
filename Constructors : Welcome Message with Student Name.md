# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
class Student:
    def __init__(self,name):
        self.a = name
    def show(self):
        print(f"Welcome {self.a}")
name = input("Enter the name of the student : ")
s = Student(name)
s.show()

## Output
<img width="1918" height="527" alt="image" src="https://github.com/user-attachments/assets/621dc9df-2aa9-4f88-9b82-69e63bc477b8" />

## Result
Thus, The Python program that creates a Student class with a default constructor and a method to display a welcome message along with the student’s name provided by the user was executed succesfully.

