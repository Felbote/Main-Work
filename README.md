# Step 1: Basic Calculator (Addition Only)
def calculate(input_str):
    num1, num2 = input_str.split('+')
    result = int(num1) + int(num2)
    return result

if __name__ == "__main__":
    user_input = input("Enter a calculation (single-digit + single-digit): ")
    result = calculate(user_input)
    print(f"The result is: {result}")

#Step 2: Advanced Calculator (All Operations)

def calculate(input_str):
    if '+' in input_str:
        num1, num2 = input_str.split('+')
        return int(num1) + int(num2)
    elif '-' in input_str:
        num1, num2 = input_str.split('-')
        return int(num1) - int(num2)
    elif '*' in input_str:
        num1, num2 = input_str.split('*')
        return int(num1) * int(num2)
    elif '/' in input_str:
        num1, num2 = input_str.split('/')
        return int(num1) / int(num2)  # This will handle float division

if __name__ == "__main__":
    user_input = input("Enter a calculation (single-digit numbers): ")
    result = calculate(user_input)
    print(f"The result is: {result}")

 #Step 3: Multi Calculator (Multiple Calculations)
def calculate(input_str):
    if '+' in input_str:
        num1, num2 = input_str.split('+')
        return int(num1) + int(num2)
    elif '-' in input_str:
        num1, num2 = input_str.split('-')
        return int(num1) - int(num2)
    elif '*' in input_str:
        num1, num2 = input_str.split('*')
        return int(num1) * int(num2)
    elif '/' in input_str:
        num1, num2 = input_str.split('/')
        return int(num1) / int(num2)


if __name__ == "__main__":
    print("Welcome to the Python calculator!")
    num_calculations = int(input("How many calculations do you want to do? "))

    for _ in range(num_calculations):
        user_input = input("What do you want to calculate? ")
        result = calculate(user_input)
        print(f"The answer is: {result}")

#Step 4: Integer Division and Remainder

def calculate(input_str):
    if '+' in input_str:
        num1, num2 = input_str.split('+')
        return int(num1) + int(num2), None
    elif '-' in input_str:
        num1, num2 = input_str.split('-')
        return int(num1) - int(num2), None
    elif '*' in input_str:
        num1, num2 = input_str.split('*')
        return int(num1) * int(num2), None
    elif '/' in input_str:
        num1, num2 = input_str.split('/')
        return int(num1) / int(num2), None
    elif '~' in input_str:
        num1, num2 = input_str.split('~')
        division = int(num1) // int(num2)
        remainder = int(num1) % int(num2)
        return division, remainder


if __name__ == "__main__":
    print("Welcome to the Python calculator!")
    num_calculations = int(input("How many calculations do you want to do? "))

    for _ in range(num_calculations):
        user_input = input("What do you want to calculate? ")
        result = calculate(user_input)

        if isinstance(result, tuple):
            print(f"The answer is: {result[0]}")
            print(f"The remainder is: {result[1]}")
        else:
            print(f"The answer is: {result}")

#Bonus Step: Support Multi-Digit Numbers

def calculate(input_str):
    if '+' in input_str:
        num1, num2 = input_str.split('+')
        return int(num1) + int(num2), None
    elif '-' in input_str:
        num1, num2 = input_str.split('-')
        return int(num1) - int(num2), None
    elif '*' in input_str:
        num1, num2 = input_str.split('*')
        return int(num1) * int(num2), None
    elif '/' in input_str:
        num1, num2 = input_str.split('/')
        return int(num1) / int(num2), None
    elif '~' in input_str:
        num1, num2 = input_str.split('~')
        division = int(num1) // int(num2)
        remainder = int(num1) % int(num2)
        return division, remainder


if __name__ == "__main__":
    print("Welcome to the Python calculator!")
    num_calculations = int(input("How many calculations do you want to do? "))

    for _ in range(num_calculations):
        user_input = input("What do you want to calculate? ")
        result = calculate(user_input)

        if isinstance(result, tuple):
            print(f"The answer is: {result[0]}")
            print(f"The remainder is: {result[1]}")
        else:
            print(f"The answer is: {result}")


