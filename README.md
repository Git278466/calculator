# Simple Calculator

# Function to perform basic arithmetic operations
def calculate(num1, num2, operation):
    if operation == '+':
        return num1 + num2
    elif operation == '-':
        return num1 - num2
    elif operation == '*':
        return num1 * num2
    elif operation == '/':
        if num2 == 0:
            return "Error! Division by zero."
        return num1 / num2
    else:
        return "Invalid operation!"

# Prompt user for inputs
try:
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    operation = input("Enter an operation (+, -, *, /): ")
    
    # Perform calculation and display result
    result = calculate(num1, num2, operation)
    print(f"Result: {result}")
except ValueError:
    print("Invalid input! Please enter numeric values.")

