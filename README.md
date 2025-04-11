# python-assignment

def calculator():
    # Prompting the user for input
    number1 = float(input("Enter the first number: "))
    number2 = float(input("Enter the second number: "))
    operation = input("Choose an operation (addition, subtraction, multiplication, division, modulus, exponentiation, floor division): ").strip().lower()

    # Performing the operation based on user choice
    if operation == "addition":
        result = number1 + number2
        print(f"The result of addition is: {result}")
    elif operation == "subtraction":
        result = number1 - number2
        print(f"The result of subtraction is: {result}")
    elif operation == "multiplication":
        result = number1 * number2
        print(f"The result of multiplication is: {result}")
    elif operation == "division":
        if number2 != 0:
            result = number1 / number2
            print(f"The result of division is: {result}")
        else:
            print("Error: Division by zero is not allowed.")
    elif operation == "modulus":
        if number2 != 0:
            result = number1 % number2
            print(f"The result of modulus is: {result}")
        else:
            print("Error: Modulus by zero is not allowed.")
    elif operation == "exponentiation":
        result = number1 ** number2
        print(f"The result of exponentiation is: {result}")
    elif operation == "floor division":
        if number2 != 0:
            result = number1 // number2
            print(f"The result of floor division is: {result}")
        else:
            print("Error: Floor division by zero is not allowed.")
    else:
        print("Invalid operation. Please choose a valid option.")

# Run the calculator function
calculator()
