# MENTAL MATH PROGRAM

# TODO LIST
- fix timer for submenu
- add subtraction
- add multiplication
- add division
- add try/catch - error handling
- add user selection
- format records.txt

category; time; problem; digits_1; digits_2
* of digits in first number, # of digits in 2nd number

 # TODO - have to figure out a way to generate ranges based on digits?
    # multiplied by 10? --- 10 raised to digit power
    # 1 digit ~ up to 9 (1 *0 to digit * 10 - 1)
    # 2 digits ~ 10 up to 99 (10^1 to 10^digit - 1)
    # 3 digits ~ 100 up to 999 (10^2 to 10^digit - 1 )

    if digit is 1: 0-9 
    generate random number(0, 10)

    else: 
    10-99
    generate random number in this range(10^(digit - 1),(10^digit))
    * don't need -1 for second digit because python doesn't include last number in range anyway

    * Fixing the timer
    https://diveintopython.org/learn/date/time
    Have to create a timer module?

    Selecting number of digits - DIGITS gets reset every time through loop

    * Need to change  it to allow for negative numbers in the same range
    - will have to adjust check for correct response
    - currently subtraction is just taking the opposite of the entry to check

    * for division - need to check if answer given is within one decimal place of correct answer (rounded)

    * for division - need to make sure you don't divide by 0
    * eventually add logarithms and exponents
    * add TTS voice for speaking problem

    TODO: fix random numbers for multiplication
    - fix digit selection (1, a) gives error
    - add in try, catch - error handling - make it so only number submissions accepted
    - add GUI
    
    Records
    Shelve - key is a string and data is any arbitrary object
    https://docs.python.org/3/library/shelve.html
    * using a temp variable is faster and uses less memory than opening dict using writeback = True

keys: A , S, M, D
(if multiple digits, sort in ascending order - 1, 2  or 2, 1 for addition -> 'A1,2')
value: list [time, n1, n2]

    - store fastest times for each operation and number of digits

    addition
    1x1
    1x2 equivalent to 2x1
    2x2 etc. 
    subtraction
    multiplication
    division