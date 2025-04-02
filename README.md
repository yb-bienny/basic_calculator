# basic_calculator
DEF function add(a, b)
    RETURN a + b

DEF function subtract(a, b)
    RETURN a - b

DEF function multiply(a, b)
    RETURN a * b

DEF function divide(a, b)
    RETURN a / b  // Ensure that b is not zero when calling

SET operations = { "+": add, "-": subtract, "*": multiply, "/": divide }

PRINT "Enter the first number:"
SET first_number = USER_INPUT

SET second_number = USER_INPUT

PRINT "Enter the operation (+, -, *, /):"
SET operation = USER_INPUT

SET result = operations[operation](first_number, second_number)

PRINT "The result of", first_number, operation, second_number, "is", result
