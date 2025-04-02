def calculator():
    print("Simple Calculator")

    # Get user input
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    operation = input("Enter an operation (+, -, *, /): ")

    # Perform the calculation
    if operation == "+":
        result = num1 + num2
    elif operation == "-":
        result = num1 - num2
    elif operation == "*":
        result = num1 * num2
    elif operation == "/":
        if num2 == 0:
            print("Error: Division by zero is not allowed.")
            return
        result = num1 / num2
    else:
        print("Error: Invalid operation. Please enter +, -, *, or /.")
        return

    # Display the result
    print(f"Result: {num1} {operation} {num2} = {result}")

# Run the calculator
calculator()

