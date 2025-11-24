# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## Algorithm

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

## Program 
```
class Calculation1:
    def Summation(self, a, b):
        return a + b

class Calculation2:
    def Subtraction(self, a, b):
        return a - b

class Derived(Calculation1, Calculation2):
    def Division(self, a, b):
        if b != 0:
            return a / b
        else:
            return "Error: Division by zero"

a = int(input())
b = int(input())
obj = Derived()

print(obj.Summation(a, b))
print(obj.Subtraction(a, b))
print(obj.Division(a, b))

```
## Output
<img width="1259" height="246" alt="image" src="https://github.com/user-attachments/assets/9a8b6ca6-5135-4c03-9b0d-ae02b27513b0" />

## Result
  Thus, the program demonstrates multiple inheritance by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes has been executed successfully.
