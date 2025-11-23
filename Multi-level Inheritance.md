# Exp.No:24  
## Multi-level Inheritance

---

### AIM  
To write a Python program to get the name, age, and ID of a person and display them using multilevel inheritance.

---

### ALGORITHM

1. Define the `Person` class:
   - Inside the `Person` class, define the `__init__` method (constructor) with two parameters: `name` and `age`.
   - Inside the `__init__` method, assign the `name` to `self.name` and `age` to `self.age`.

2. Define the `PersonDetails` class that inherits from the `Person` class:
   - Inside the `PersonDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `Person` class using `super()` to initialize `name` and `age`.
   - Assign `person_id` to `self.person_id`.

3. Define the `DisplayDetails` class that inherits from the `PersonDetails` class:
   - Inside the `DisplayDetails` class, define the `__init__` method (constructor) with three parameters: `name`, `age`, and `person_id`.
   - Inside the `__init__` method, call the `__init__` method of the `PersonDetails` class using `super()` to initialize `name`, `age`, and `person_id`.

4. Inside the `DisplayDetails` class, define the `show_details` method:
   - Inside the `show_details` method, return a formatted string with `self.name`, `self.age`, and `self.person_id`.

5. Prompt the user to enter `name` (string), `age` (integer), and `person_id` (integer).

6. Create an instance `person` of the `DisplayDetails` class, passing `name`, `age`, and `person_id` to the constructor.

7. Call the `show_details` method on the `person` object and print the result.

8. Terminate the program.

---

### PROGRAM

```python
class Person_name:
    def get_name(self,name):
        self.name=name
        
class Person_age(Person_name):
    def get_age(self,age):
        self.age=age
        
class Person_salary(Person_age):
    def get_salary(self,salary):
        self.salary=salary
        
    def display(self):
        print(self.name, self.age, self.salary)
        
name=input()
age=input()
salary=input()

p=Person_salary()
p.get_name(name)
p.get_age(age)
p.get_salary(salary)
p.display()

```
---
### OUTPUT

<img width="1255" height="214" alt="image" src="https://github.com/user-attachments/assets/6c984907-3126-4c0a-b74e-ddf62e748c49" />

---
### RESULT
Thus the Python program to get the name, age, and ID of a person and display them using multilevel inheritance was implemented and executed successfully.
