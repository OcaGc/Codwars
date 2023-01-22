<h2>Instructions:</h2>

In this little assignment you are given a string of space separated numbers, and have to return the highest and lowest number.

<h2>Examples:</h2>

high_and_low("1 2 3 4 5")  # return "5 1"
high_and_low("1 2 -3 4 5") # return "5 -3"
high_and_low("1 9 3 4 -5") # return "9 -5"

<h2>Notes:</h2>

All numbers are valid Int32, no need to validate them.
There will always be at least one number in the input string.
Output string must be two numbers separated by a single space, and highest number is first.

<h2>Given code:</h2>

def high_and_low (numbers):
 # ...
    return numbers
    
_________________________________________________________________________________________________________________________________

<h2>Solution:</h2>

def high_and_low(numbers):
    numbers = sorted(list(map(int, numbers.split())))
    return f'{max(numbers)} {min(numbers)}'
