def calculator():

    number_1 = float(input("please enter your number:\n"))
    number_2 = float(input("please enter your number:\n"))

    operation = input('''
    Please enter the action you want to do with the calculator:
    + for addition
    - for subtraction
    * for multiplication
    / for division
    % for residue
    // For tribute part
    ** for exponent
    ''')
    if operation == "+":
        output_number = number_1 + number_2
        print("{} + {} = {}" . format(number_1 ,number_2 , output_number))
    elif operation == "-":
        output_number = number_1 - number_2
        print("{} - {} = {}". format(number_1 , number_2 , output_number))
    elif operation == "*":
        output_number = number_1 * number_2
        print("{} * {} = {}". format(number_1 , number_2 , output_number))
    elif operation == "/":
        output_number = number_1 - number_2
        print("{} / {} = {}". format(number_1 , number_2 , output_number))
    elif operation == "%":
        output_number = number_1 - number_2
        print("{} % {} = {}". format(number_1 , number_2 , output_number))
    elif operation == "//":
        output_number = number_1 // number_2
        print("{} // {} = {}". format(number_1 , number_2 , output_number))
    elif operation == "**":
        output_number = number_1 ** number_2
        print("{} ** {} = {}". format(number_1 , number_2 , output_number))
    else:
        print('You have not typed a valid operator, please run the program again.')
        
def again():
    calculator_again = input('''
    Do you want to calculate again?
    Please type Y for YES or N for NO.\n
    ''')
    if calculator_again.upper == "Y":
        calculator()
    elif calculator_again.upper == "N":
        print("see you later.")
    else:
        again()

calculator()
again()
