# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
class detail:
    def __init__(self):
        self.name = input()
        self.age = input()
class Employee(detail):
    def getEmployeeDetail(self):
        self.ID = input()
        self.department = input()
    def show(self):
        print("Name Of The Employee : ",self.name)
        print("Age Of The Employee : ",self.age)
        print("ID Of The Employee : ",self.ID)
        print("Department Of The Employee : ",self.department)
class Patient(detail):
    def getPatientDetail(self):
        self.ID = input()
        self.disease = input()
    def show(self):
        print("Name Of The Patient : ",self.name)
        print("Age Of The Patient : ",self.age)
        print("ID Of The Patient : ",self.ID)
        print("Disease Of The Patient : ",self.disease)
print("Enter the Employee Details.....")
emp = Employee()
emp.getEmployeeDetail()
emp.show()
print("\nEnter the Patient Details.....")
pat = Patient()
pat.getPatientDetail()
pat.show()
## Sample Output
<img width="1917" height="802" alt="image" src="https://github.com/user-attachments/assets/7a968507-de62-4210-8005-231a6af48b2d" />

## Result
Thus, The Python program that uses Hierarchical Inheritance to input and display Employee and Patient details was executed successfully.
