import operator
from operator import add, sub

# Q1: A Plus Abs B
# Fill in the blanks in the following function for adding a to the absolute value of b, without calling abs.
# You may not modify any of the provided code other than the two blanks.
def a_plus_abs_b(a, b):
    """Return a+abs(b), but without calling abs.

    >>> a_plus_abs_b(2, 3)
    5
    >>> a_plus_abs_b(2, -3)
    5
    >>> a_plus_abs_b(-1, 4)
    3
    >>> a_plus_abs_b(-1, -4)
    3
    """
    if b < 0:
        f = operator.sub
    else:
        f = operator.add
    return f(a, b)


# Q2: Two of Three
# Write a function that takes three positive numbers as arguments and returns
# the sum of the squares of the two smallest numbers.
# Use only a single line for the body of the function.
def two_of_three(i, j, k):
    """Return m*m + n*n, where m and n are the two smallest members of the
    positive numbers i, j, and k.

    >>> two_of_three(1, 2, 3)
    5
    >>> two_of_three(5, 3, 1)
    10
    >>> two_of_three(10, 2, 8)
    68
    >>> two_of_three(5, 5, 5)
    50
    """
    return i*i + j*j + k*k - max(i,j,k)*max(i,j,k)


# Q3: Largest Factor
# Write a function that takes an integer n that is greater than 1 and
# returns the largest integer that is smaller than n and evenly divides n.
def largest_factor(n):
    """Return the largest factor of n that is smaller than n.

    >>> largest_factor(15) # factors are 1, 3, 5
    5
    >>> largest_factor(80) # factors are 1, 2, 4, 5, 8, 10, 16, 20, 40
    40
    >>> largest_factor(13) # factor is 1 since 13 is prime
    1
    >>> largest_factor(180)
    90
    """
    assert isinstance(n, int), 'n needs to be an integer'
    assert n > 1, 'n should be larger than 1'
    i = n
    while i > 0:
        i = i - 1
        if n % i == 0:
            return i


# Q4 Hailstone
# Write a function that takes a single argument with formal parameter name n,
# prints out the hailstone sequence starting at n, and returns the number of steps in the sequence
# Rules:
# Pick a positive integer n as the start.
# If n is even, divide it by 2.
# If n is odd, multiply it by 3 and add 1.
# Continue this process until n is 1.
def hailstone(n):
    """Print the hailstone sequence starting at n and return its
    length.

    >>> a = hailstone(10)
    10
    5
    16
    8
    4
    2
    1
    >>> a
    7
    >>> b = hailstone(1)
    1
    >>> b
    1
    """
    "*** YOUR CODE HERE ***"
    assert n >= 1, 'n needs to be larger than or equal to 1'

    if n == 1:
        i = 1

    i = 1
    while n > 1:
        print(n)
        if n % 2 == 0:
            n = n // 2
        else:
            n = n * 3 + 1
        i += 1
    print(n)
    return i
