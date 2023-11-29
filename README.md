# Hello-software-class
In this Assignment we are paired to understand the git, uses of git, features in git.

##code 
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y != 0:
        return x / y
    else:
        print("Error: Division by zero")
        return None

def calculator():
    print("Simple Calculator")
    while True:
        try:
            num1 = float(input("Enter the first number: "))
            operation = input("Enter the operation (+, -, *, /): ")
            num2 = float(input("Enter the second number: "))

            if operation == '+':
                result = add(num1, num2)
            elif operation == '-':
                result = subtract(num1, num2)
            elif operation == '*':
                result = multiply(num1, num2)
            elif operation == '/':
                result = divide(num1, num2)
            else:
                print("Error: Invalid operation")
                continue

            print("Result: {}".format(result))

            cont = input("Do you want to perform another calculation? (y/n): ")
            if cont.lower() != 'y':
                print("Exiting the calculator. Goodbye!")
                break
        except ValueError:
            print("Error: Invalid input. Please enter valid numbers.")
        except Exception as e:
            print(f"An error occurred: {str(e)}")

if __name__ == "__main__":
    calculator()


####This calculator program allows the user to perform basic arithmetic operations (+, -, *, /) on two numbers. It includes error handling for invalid inputs and division by zero. 
