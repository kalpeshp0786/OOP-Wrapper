# Employee Management System

## Project Overview

Employee Management System is a simple Python OOP project created to understand and implement Object-Oriented Programming concepts.

This project allows the user to create and display details of different types of people and employees using a menu-driven system.

The project contains four classes:

* Person
* Employee
* Manager
* Developer

The `Employee` class inherits from the `Person` class, while `Manager` and `Developer` inherit from the `Employee` class.

## Objectives

The main objectives of this project are:

* To understand Python classes and objects.
* To understand inheritance.
* To use constructors in classes.
* To implement encapsulation.
* To use getter and setter methods.
* To understand method overriding.
* To use the `super()` function.
* To understand the destructor method.
* To create a simple menu-driven Python program.

## Project Features

The program provides the following options:

1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Exit

## Class Structure

### 1. Person Class

The `Person` class is the parent class.

It contains:

* Name
* Age
* `display()` method
* `__del__()` destructor

Example:

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age
```

### 2. Employee Class

The `Employee` class inherits from the `Person` class.

It contains:

* Employee ID
* Salary
* Getter methods
* Setter methods
* `display()` method

Employee ID and salary are private variables:

```python
self.__employee_id
self.__salary
```

The class uses getter and setter methods to access and modify these values.

### 3. Manager Class

The `Manager` class inherits from the `Employee` class.

It contains an additional:

* Department

The `display()` method is overridden to show the department details.

### 4. Developer Class

The `Developer` class also inherits from the `Employee` class.

It contains an additional:

* Programming Language

The `display()` method is overridden to show the programming language.

## OOP Concepts Used

### Class and Object

The project uses classes to define Person, Employee, Manager, and Developer.

Objects are created using these classes.

```python
person_obj = Person(name, age)
employee_obj = Employee(name, age, emp_id, salary)
```

### Inheritance

Inheritance is used between the classes.

```text
Person
   |
Employee
   |
   +-------- Manager
   |
   +-------- Developer
```

### Encapsulation

Employee ID and salary are stored as private variables:

```python
self.__employee_id
self.__salary
```

Getter and setter methods are used to access and modify them.

### Constructor

The `__init__()` method is used to initialize object data.

```python
def __init__(self, name, age):
```

### Method Overriding

The `display()` method is defined in the parent class and overridden in the child classes.

For example:

```python
def display(self):
    super().display()
    print(f"Department: {self.department}")
```

### super()

The `super()` function is used to call the parent class constructor and methods.

Example:

```python
super().__init__(name, age)
```

### Destructor

The project uses the `__del__()` method.

```python
def __del__(self):
    pass
```

## Program Menu

When the program starts, the following menu is displayed:

```text
Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Exit
```

### Create a Person

The user enters:

* Name
* Age

A Person object is created.

### Create an Employee

The user enters:

* Name
* Age
* Employee ID
* Salary

An Employee object is created.

### Create a Manager

The user enters:

* Name
* Age
* Employee ID
* Salary
* Department

A Manager object is created.

### Create a Developer

The user enters:

* Name
* Age
* Employee ID
* Salary
* Programming Language

A Developer object is created.

### Show Details

The program provides another menu:

```text
Choose details to show:
1. Person
2. Employee
3. Manager
4. Developer
```

The user can select which object's details they want to display.

### Exit

Option 6 exits the program.

```text
Exiting the system. All resources have been freed!

Goodbye!
```

## Sample Output

```text
--- Python OOP Project: Employee Management System ---

Choose an operation:
1. Create a Person
2. Create an Employee
3. Create a Manager
4. Create a Developer
5. Show Details
6. Exit

Enter your choice: 1
Enter Name: Mihir Patel
Enter Age: 25

Person created with name: Mihir Patel and age: 25.

--- Choose another operation ---

Enter your choice: 2
Enter Name: Jainil Vyash
Enter Age: 23
Enter Employee ID: E786
Enter Salary: 40000

Employee created with name: Jainil Vyash, age: 23, ID: E786, and salary: $40000.0.

--- Choose another operation ---

Enter your choice: 3
Enter Name: Alice Johnson
Enter Age: 40
Enter Employee ID: M420
Enter Salary: 60000
Enter Department: 3

Manager created with name: Alice Johnson, age: 40, ID: M420, salary: $60000.0, and department: 3.

--- Choose another operation ---

Enter your choice: 4
Enter Name: Jane Smith
Enter Age: 45
Enter Employee ID: V008
Enter Salary: 80000
Enter Programming Language: Python, Java Etc.

Developer created with name: Jane Smith, age: 45, ID: V008, salary: $80000.0, and programming language: Python, Java Etc..

--- Choose another operation ---

Enter your choice: 5

Choose details to show:
1. Person
2. Employee
3. Manager
4. Developer

Enter your choice: 2

Name: Jainil Vyash
Age: 23
Employee ID: E786
Salary: $40000.0

Enter your choice: 6

Exiting the system. All resources have been freed!

Goodbye!
```

## Technologies Used

* Python
* Object-Oriented Programming
* Python Classes and Objects
* Inheritance
* Encapsulation
* Getter and Setter Methods
* Method Overriding

## Project Structure

```text
Employee-Management-System/
│
├── employee_management.py
└── README.md
```

## How to Run

### Step 1: Install Python

Make sure Python is installed on your computer.

Check the Python version:

```bash
python --version
```

### Step 2: Save the Code

Save the given Python code in a file such as:

```text
employee_management.py
```

### Step 3: Run the Program

Open the terminal in the project folder and run:

```bash
python employee_management.py
```

### Step 4: Use the Menu

Enter the option number according to the operation you want to perform.

## Input Details

| Class     | Input                                                |
| --------- | ---------------------------------------------------- |
| Person    | Name, Age                                            |
| Employee  | Name, Age, Employee ID, Salary                       |
| Manager   | Name, Age, Employee ID, Salary, Department           |
| Developer | Name, Age, Employee ID, Salary, Programming Language |

## Learning Outcomes

After completing this project, I learned:

* How to create Python classes and objects.
* How inheritance works in Python.
* How to use private variables.
* How getter and setter methods work.
* How to override methods.
* How to use `super()`.
* How constructors and destructors work.
* How to create a menu-driven program.
* How different classes can be connected using inheritance.

## Conclusion

The Employee Management System is a simple Python project created using Object-Oriented Programming concepts.

It demonstrates classes, objects, inheritance, encapsulation, method overriding, constructors, getters, setters, `super()`, and destructors in a practical way.

This project helped in understanding the basic concepts of Python OOP through a simple employee management system.

## Author

Meet Prajapati
