# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
from abc import ABC
class Shape(ABC):
    def calculate_area(self):
        pass
class Rectangle(Shape):
    length = 5
    breadth =3 
    def calculate_area(self):
        return self.length * self.breadth

class Circle(Shape):
  radius = 4
  def calculate_area(self):
        return self.radius * self.radius*3.14

rec=Rectangle()
cir=Circle()

print("Area of a rectangle:", rec.calculate_area())
print("Area of a circle:", cir.calculate_area())
```
## Output
<img width="1920" height="1080" alt="Screenshot (135)" src="https://github.com/user-attachments/assets/70f4edc0-902d-4d95-8df2-438702991d95" />

## Result
Thus, the program is executed successfully.
# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
class Rectangle:
    def __init__(self, length, width):
        self.__length = length  
        self.__width = width    
    
    
    def print_values(self):
        print("Length is ",self.__length)
        print("Width is ",self.__width)


rect = Rectangle(5, 3)


rect.print_values()
```
## Output
<img width="1920" height="1080" alt="Screenshot (136)" src="https://github.com/user-attachments/assets/7152eac1-aa87-45af-a3b9-1703838c779c" />

## Result
Thus, the program is executed successfully.
# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

## 💻 PROGRAM:
```
class Fish:
    def type(self):
        print("fish")


class Shark(Fish):
    def type(self):
        print("shark")


obj_goldfish = Fish()
obj_hammerhead = Shark()

obj_goldfish.type()
obj_hammerhead.type()
```
## OUTPUT
<img width="1920" height="1080" alt="Screenshot (137)" src="https://github.com/user-attachments/assets/32a7a09b-b2ec-4cae-b47e-4e6311bd56c0" />

## RESULT
Thus, the program is executed successfully.
# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program
```
class A:
    def __init__(self,a):
        self.a=a
    def __gt__(self,other):
        return self.a<other.a
ob1=A(200)
ob2=A(30)
if(ob1<ob2):
    print("ob2 is less than ob1")
else:
    print("ob1 is less than ob1")
```
## Output
<img width="1920" height="1080" alt="Screenshot (138)" src="https://github.com/user-attachments/assets/1dde1526-6d58-42d8-abd1-faed4323d17c" />

## Result
Thus, the program is executed successfully.
