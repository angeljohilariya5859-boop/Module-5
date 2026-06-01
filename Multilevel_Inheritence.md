# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
class Parents:
    def __init__(self,name):
        self.name = name
    def getName(self):
        print("Name : ",self.name)
class Child(Parents):
    def __init__(self,name,age):
        super().__init__(name)
        self.age = age
    def getAge(self):
        print("Age : ",self.age)
class Grandchild(Child):
    def __init__(self,name,age,location):
        super().__init__(name,age)
        self.loc = location
    def getLocation(self):
        print("Location : ",self.loc)
name = input("Enter Your Name : ")
age = int(input("Enter Your Age : "))
location = input("Enter Your Location : ")
get = Grandchild(name,age,location)
print("\nThe User Details.....")
get.getName()
get.getAge()
get.getLocation()

## Sample Output
<img width="1292" height="906" alt="image" src="https://github.com/user-attachments/assets/58d33a28-1e5e-4a2a-a2fc-021b607ba86e" />
## Result
Thus, The Python program that uses multilevel inheritance to get and display a person’s name, age, and location was executed sucessfully.
