add = lambda x, y: x + y
subtraction = lambda x, y: x - y
multiplication = lambda x, y: x * y
division = lambda x, y: x / y if y != 0 else "Error: Division by zero"

print(":::::::SIMPLE CALCULATOR::::::::")
print("Select an arithmetic operator")
print("1. +")
print("2. -")
print("3. *")
print("4. /")
operator = input("Enter an arithmetic operator (+, -, *, /): ")
try:
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    if operator == "+":
        print(f"Result: {add(num1, num2)}")
    elif operator == "-":
        print(f"Result: {subtraction(num1, num2)}")
    elif operator == "*":
        print(f"Result: {multiplication(num1, num2)}")
    elif operator == "/":
        print(f"Result: {division(num1, num2)}")
    else:
        print("Invalid operator")
except ValueError:
    print("Invalid input. Please enter numeric values.")