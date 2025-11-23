# Exp.No:22  
## Destructor

---

### AIM  
To create a Python class `Student` with a destructor.

---

### ALGORITHM

1. Begin the program.  
2. Define the `student` class.  
3. Inside the `student` class, define the `__init__` method (constructor) and the `__del__` method (destructor).  
4. Create an object `s2` of the `student` class. When the object `s2` is created, the `__init__` method is called, and its print statements are executed.  
5. Use the `del` statement to delete the object `s2`. This triggers the `__del__` method (destructor), and the respective print statements are executed.  
6. Terminate the program.

---

### PROGRAM

```python
class Student:
    def __init__(self,name):
        self.name=name
        print("Inside Constructor")
        print("Object initialized")
        print(f"Hello, my name is {self.name}")
        
    def __del__(self):
        print("Inside destructor")
        print("Object destroyed")
        
obj=Student("Emma")
del obj
```
---
### OUTPUT

<img width="938" height="260" alt="image" src="https://github.com/user-attachments/assets/718c7e2a-700e-4a7e-b5d2-aab5fc048074" />

---
### RESULT

Thus the Python class Student with a destructor was implemented and executed successfully.
