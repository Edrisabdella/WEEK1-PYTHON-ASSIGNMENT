# Basic Calculator - Python CLI
# Author: Edris Abdella
# Ask the user to input two numbers and a mathematical operation
import sys
try:
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
except ValueError:
    print("Error: Please enter valid numbers.")
    sys.exit()
operation = input("Enter an operation (+, -, *, /): ")

# Perform the chosen operation
if operation == "+":
    result = num1 + num2
    print(f"{num1} + {num2} = {result}")
elif operation == "-":
    result = num1 - num2
    print(f"{num1} - {num2} = {result}")
elif operation == "*":
    result = num1 * num2
    print(f"{num1} * {num2} = {result}")
elif operation == "/":
    if num2 != 0:
        result = num1 / num2
        print(f"{num1} / {num2} = {result}")
    else:
        print("Error: Division by zero is not allowed.")
else:
    print("Invalid operation. Please choose from +, -, *, /.")
# End of calculator script
# Save this script as my_calculator.py and run it in a Python environment.
