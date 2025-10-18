import math

# 1. Square: Perimeter and Area
side = float(input("Enter the side of the square: "))
square_perimeter = 4 * side
square_area = side ** 2
print(f"Square - Perimeter: {square_perimeter}, Area: {square_area}")

# 2. Circle: Circumference from Diameter
diameter = float(input("Enter the diameter of the circle: "))
circle_circumference = math.pi * diameter
print(f"Circle - Circumference: {circle_circumference}")

# 3. Mean of two numbers
a = float(input("Enter the first number (a): "))
b = float(input("Enter the second number (b): "))
mean = (a + b) / 2
print(f"Mean of {a} and {b} is {mean}")

# 4. Sum, Product, and Squares
sum_ab = a + b
product_ab = a * b
square_a = a ** 2
square_b = b ** 2
print(f"Sum: {sum_ab}")
print(f"Product: {product_ab}")
print(f"Square of {a}: {square_a}")
print(f"Square of {b}: {square_b}")


