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
# Base Class
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

# Derived Class 1
class Employee(Person):
    def __init__(self, name, age, emp_id, salary):
        super().__init__(name, age)
        self.emp_id = emp_id
        self.salary = salary

    def display_employee(self):
        print("\nEmployee Details")
        print("Name :", self.name)
        print("Age :", self.age)
        print("Employee ID :", self.emp_id)
        print("Salary :", self.salary)

# Derived Class 2
class Patient(Person):
    def __init__(self, name, age, patient_id, disease):
        super().__init__(name, age)
        self.patient_id = patient_id
        self.disease = disease

    def display_patient(self):
        print("\nPatient Details")
        print("Name :", self.name)
        print("Age :", self.age)
        print("Patient ID :", self.patient_id)
        print("Disease :", self.disease)

# Input Employee Details
ename = input("Enter Employee Name: ")
eage = int(input("Enter Employee Age: "))
emp_id = input("Enter Employee ID: ")
salary = float(input("Enter Salary: "))

emp = Employee(ename, eage, emp_id, salary)

# Input Patient Details
pname = input("\nEnter Patient Name: ")
page = int(input("Enter Patient Age: "))
patient_id = input("Enter Patient ID: ")
disease = input("Enter Disease: ")

pat = Patient(pname, page, patient_id, disease)

# Display Details
emp.display_employee()
pat.display_patient()

## Sample Output
<img width="1917" height="802" alt="image" src="https://github.com/user-attachments/assets/7a968507-de62-4210-8005-231a6af48b2d" />

## Result
Thus, The Python program that uses Hierarchical Inheritance to input and display Employee and Patient details was executed successfully.
