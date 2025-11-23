# Exp.No:23  
## Multiple Inheritance

---

### AIM  
To write a Python program to get the name, attendance, and ID of a student and check if they are eligible for the next module using multiple inheritance. If attendance > 80, the student is eligible; otherwise, not eligible.

---

### ALGORITHM

1. Define the `Student` class.
2. Inside the `Student` class, define the `__init__` method (constructor). The `__init__` method accepts two parameters: `name` and `student_id`.
    - Inside the `__init__` method: Assign the value of `name` to `self.name` and `student_id` to `self.student_id`.
3. Define the `get_student_info` method inside the `Student` class:
    - This method should return a string formatted with `self.name` and `self.student_id`.
4. Define the `Attendance` class, which inherits from the `Student` class.
5. Inside the `Attendance` class, define the `__init__` method (constructor).
    - The `__init__` method accepts three parameters: `name`, `student_id`, and `attendance`.
    - Inside the `__init__` method: Call the parent class constructor `super().__init__(name, student_id)` to initialize `name` and `student_id`. Assign the value of `attendance` to `self.attendance`.
6. Define the `check_eligibility` method inside the `Attendance` class:
    - If `self.attendance` is greater than 80, return a formatted string indicating the student is eligible for the module exam.
    - Otherwise, return a formatted string indicating the student is not eligible for the module exam.
7. Prompt the user to enter the `name` (as a string), `student_id` (as an integer), and `attendance` (as an integer).
8. Create an instance `student` of the `Attendance` class, passing the entered `name`, `student_id`, and `attendance` to the constructor.
9. Call the `check_eligibility` method on the `student` object and print the result.
10. Terminate the program.

---

### PROGRAM

```python
class StudentInfo:
    def get_info(self, name, student_id):
        self.name = name
        self.student_id = student_id

class Attendance:
    def get_attendance(self, attendance):
        self.attendance = attendance

class ExamEligibility(StudentInfo, Attendance):
    def check_eligibility(self):
        print(self.name)
        print(self.student_id)
        if self.attendance > 75:
            print("Eligible for Exam")
        else:
            print("Not Eligible for Exam")


# First student
name1 = input()
id1 = int(input())
att1 = int(input())

student1 = ExamEligibility()
student1.get_info(name1, id1)
student1.get_attendance(att1)
student1.check_eligibility()

```

---
### OUTPUT

<img width="940" height="297" alt="image" src="https://github.com/user-attachments/assets/582c398a-5dc3-4f7e-b986-157754b54995" />

---
### RESULT

Thus the Python program to get the name, attendance, and ID of a student and check if they are eligible for the next module using multiple inheritance. If attendance > 80, the student is eligible; otherwise, not eligible was implemented and executed successfully.






