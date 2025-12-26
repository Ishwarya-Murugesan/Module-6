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
