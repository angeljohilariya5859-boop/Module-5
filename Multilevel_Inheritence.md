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
# Base Class
class Person:
    def get_name(self):
        self.name = input("Enter Name: ")

# Derived Class 1
class Age(Person):
    def get_age(self):
        self.age = int(input("Enter Age: "))

# Derived Class 2
class Location(Age):
    def get_location(self):
        self.location = input("Enter Location: ")

    def display(self):
        print("\nPerson Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Location:", self.location)

# Object Creation
obj = Location()

# Input Details
obj.get_name()
obj.get_age()
obj.get_location()

# Display Details
obj.display()

## Sample Output

<img width="1292" height="906" alt="image" src="https://github.com/user-attachments/assets/58d33a28-1e5e-4a2a-a2fc-021b607ba86e" />
## Result

Thus, The Python program that uses multilevel inheritance to get and display a person’s name, age, and location was executed sucessfully.
