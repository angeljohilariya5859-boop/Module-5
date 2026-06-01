# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
# Base Class 1
class Add:
    def addition(self, a, b):
        return a + b

# Base Class 2
class Sub:
    def subtraction(self, a, b):
        return a - b

# Derived Class (inherits from Add and Sub)
class Division(Add, Sub):
    def division(self, a, b):
        return a / b

# Object Creation
obj = Division()

# Input
a = float(input("Enter First Number: "))
b = float(input("Enter Second Number: "))

# Output
print("Addition =", obj.addition(a, b))
print("Subtraction =", obj.subtraction(a, b))
print("Division =", obj.division(a, b))

## Output Example

<img width="1917" height="916" alt="image" src="https://github.com/user-attachments/assets/7478d64c-b4bd-4bb7-a68c-f1c4b3af5dea" />

## Result

Thus, The Python program demonstrates multiple inheritance by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes was executed successfully.

