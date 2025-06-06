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
    def __init__(self, length, breadth):
        self.__length = length
        self.__breadth = breadth

    def set_length(self, length):
        self.__length = length

    def get_length(self):
        return self.__length

    def set_breadth(self, breadth):
        self.__breadth = breadth

    def get_breadth(self):
        return self.__breadth

    def calculate_area(self):
        return self.__length * self.__breadth

rect = Rectangle(10, 5)
print("Length:", rect.get_length())
print("Breadth:", rect.get_breadth())
print("Area:", rect.calculate_area())
```

## Output
```
Length: 10
Breadth: 5
Area: 50
```

## Result
The program demonstrates encapsulation by keeping the member variables __length and __breadth private and providing public getter and setter methods to access and modify them safely.
