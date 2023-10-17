# cousera-google-python-module-3-graded-test
#QUESTION 1
number = 2 # Initialize the variable 
while number <= 12: # Complete the while loop condition
    print(number, end=" ")
    number += 2 # Increment the variable

# Should print 2 4 6 8 10 12

QUESTION 2
for number in range(5):
    if number % 2 == 1:
        print("even")
    else:
        print("odd")


# Should print:
# odd
# even
# odd
# even
# odd

QUESTION 3
def even_numbers(n):
    count = 0
    current_number = 0
    while current_number <= n: # Complete the while loop condition
        if current_number % 2 == 0:
            count += 1 # Increment the appropriate variable
        current_number += 1 # Increment the appropriate variable
    return count
    
print(even_numbers(25))   # Should print 13
print(even_numbers(144))  # Should print 73
print(even_numbers(1000)) # Should print 501
print(even_numbers(0))    # Should print 1

QUESTION 4
def sequence(low, high):
    # Complete the outer loop range to make the loop run twice
    # to create two rows
    for x in range(2): 
        # Complete the inner loop range to print the given variable
        # numbers starting from "high" to "low" 
        # Hint: To decrement a range parameter, use negative numbers
        for y in range(high, low-1, -1): 
            if y == low:
                # Don’t print a comma after the last item
                print(str(y)) 
            else:
                # Print a comma and a space between numbers
                print(str(y), end=", ") 

sequence(1, 3)
# Should print the sequence 3, 2, 1 two times, as shown above.

QUESTION 5
def divisible(max, divisor):
    count = 0 # Initialize an incremental variable
    for x in range(1, max+1): # Complete the for loop
        if x % divisor == 0:
            count += 1 # Increment the appropriate variable
    return count

print(divisible(100, 10)) # Should be 10
print(divisible(10, 3)) # Should be 3
print(divisible(144, 17)) # Should be 8

QUESTION 6
def even_numbers(maximum):
    return_string = ""  # Initializes variable as an empty string

    # Complete the for loop with a range that includes all even numbers
    # up to and including the "maximum" value, but excluding 0.
    for num in range(2, maximum + 1):

        # Complete the body of the loop by appending the even number
        # followed by a space to the "return_string" variable.
        if num % 2 == 0:
            return_string += str(num) + " "

    # This .strip command will remove the final " " space at the end of
    # the "return_string".
    return return_string.strip()

print(even_numbers(6))  # Should be 2 4 6
print(even_numbers(10))  # Should be 2 4 6 8 10
print(even_numbers(1))   # No numbers displayed
print(even_numbers(3))   # Should be 2
print(even_numbers(0))   # No numbers displayed

QUESTION 7
x = 1
sum = 5
while x <= 10:
    sum += x
    x += 1
print(sum)
# Should print 55
