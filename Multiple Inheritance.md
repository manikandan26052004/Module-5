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
```
REG NO: 212222220022
NAME: MANIKANDAN R
class one():
    def student1(self,name,att,id):
        print(name)
        print(att)
        print("Eligible for Module Exam")
class two():
    def student2(self,name,att,id):
        print(name)
        print(att)
        print("Not Eligible for Module Exam")
class valid(one,two):
    def valid(self,name,att,id):
        if id>75:
            one().student1(name,att,id)
        else:
            two().student2(name,att,id)
name=input()
att=int(input())
id=int(input())
x=valid()
x.valid(name,att,id)
```

### OUTPUT


![MODULE 5E](https://github.com/user-attachments/assets/5f3b3393-f99f-4d29-958b-e9ad4bdc3852)


### RESULT
This program for  get the name, attendance, and ID of a student and check if they are eligible for the next module using multiple inheritance. If attendance > 80, the student is eligible; otherwise, not eligible is successfuly executed. 
