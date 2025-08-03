# CALCULATOR
 # Write a python program to build a simple  Calculator-

# 3 steps to build calculator program
# 1-function for opertions
# 2-user input
# 3-print result

# Available Operation
# 1- "Addition(1): Sum of multiple numbers."
# 2- "Substraction(2): Diffrence between two numbers."
# 3- "Multiplication (3): product of multiple between two numbers."
# 4- "Division (4): Quotient of two numbers."
# 5- "Average (5): Aevrage of multiple numbers."

# step-1 Create Functions-
# function to add two numbers
def add(num1,num2):
    return num1 + num2

# function to subsrtrct two numbers
def sub(num1,num2):
    return num1 - num2

# function multiply two numbers
def multiply(num1,num2):
    return num1 * num2

#function divide two numbers
def divide(num1,num2):
    return num1 / num2

#function average two numbers
def avg(num1,num2):
    return (num1 + num2)/2

# step-2 User input
print("Please select a operation:\n " \
    "1. Addition\n" \
    "2.Substraction\n" \
    "3.Multiply\n" \
    "4.Divide\n" \
    "5. Aevrage\n")

select = int(input("Select a operation from 1,2,3,4,5: "))

number1 = int(input("Enter first number:"))
number2= int(input("Enter second number:"))

# step-3 Print the result

if select == 1:
    print(number1, "+", number2, "=", \
        add(number1, number2))
    
elif select == 2:
    print(number1, "-", number2, "=", \
        sub(number1, number2))

elif select == 3:
    print(number1, "*", number2, "=", \
        multiply(number1, number2))
    
elif select == 4:
    print(number1, "/", number2, "=", \
        divide(number1, number2))    
    
elif select == 5:
    print("(",number1, "+", number2, ")", "/", "2", "=", \
        avg(number1, number2)) 

else:
    print("Invalid operation1! pls select again!")          
