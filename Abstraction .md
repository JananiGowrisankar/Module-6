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
from abc import ABC, abstractmethod
import math

# Step 2: Create Abstract Class
class Shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass

# Step 3: Subclass Rectangle
class Rectangle(Shape):
    def __init__(self, length=5, breadth=3):
        self.length = length
        self.breadth = breadth

    def calculate_area(self):
        area = self.length * self.breadth
        print(f"Rectangle Area: {area}")

# Step 4: Subclass Circle
class Circle(Shape):
    def __init__(self, radius=4):
        self.radius = radius

    def calculate_area(self):
        area = math.pi * self.radius ** 2
        print(f"Circle Area: {area:.2f}")

# Step 5: Create Objects & Call Methods
rect = Rectangle()
circ = Circle()

rect.calculate_area()
circ.calculate_area()

```

## Output

![image](https://github.com/user-attachments/assets/f8b149f5-b361-47c5-bdfe-5e992e548b8c)

## Result
Thus the python program is successfully verified.
## Result
