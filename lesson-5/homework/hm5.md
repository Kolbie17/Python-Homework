def is_leap(year):
    """
    Determines whether a given year is a leap year.

    A year is a leap year if:
    - It is divisible by 4, and
    - It is NOT divisible by 100, unless it is also divisible by 400.

    Parameters:
        year (int): The year to be checked.

    Returns:
        bool: True if the year is a leap year, False otherwise.
    """
    if not isinstance(year, int):
        raise ValueError("Year must be an integer.")

    return (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0)


n = int(input("Enter an integer: "))

if n % 2 != 0:
    print("Weird")
elif n % 2 == 0 and 2 <= n <= 5:
    print("Not Weird")
elif n % 2 == 0 and 6 <= n <= 20:
    print("Weird")
elif n % 2 == 0 and n > 20:
    print("Not Weird")

# Input Format: A single line containing a positive integer, n.
n = int(input().strip())

if n % 2 != 0:
    print("Weird")
elif 2 <= n <= 5:
    print("Not Weird")
elif 6 <= n <= 20:
    print("Weird")
else:
    print("Not Weird")
n = int(input().strip())

if n % 2 != 0:
    print("Weird")
elif 2 <= n <= 5:
    print("Not Weird")
elif 6 <= n <= 20:
    print("Weird")
elif n > 20:
    print("Not Weird")

n = int(input().strip())

if n % 2 != 0:
    print("Weird")
elif 2 <= n <= 5:
    print("Not Weird")
elif 6 <= n <= 20:
    print("Weird")
else:
    print("Not Weird")


# Read a single integer from input
n = int(input().strip())

# Conditional logic
if n % 2 != 0:
    print("Weird")
elif 2 <= n <= 5:
    print("Not Weird")
elif 6 <= n <= 20:
    print("Weird")
else:
    print("Not Weird")

a = int(input("Enter a: "))
b = int(input("Enter b: "))

# Make sure a <= b
if a > b:
    a, b = b, a

# Use range() with step 2 — no loop explicitly written
start = a if a % 2 == 0 else a + 1
evens = list(range(start, b + 1, 2))
print(evens)


a = int(input("Enter a: "))
b = int(input("Enter b: "))

# Ensure a <= b automatically
a, b = min(a, b), max(a, b)

# One-liner using math
evens = list(range(a + a % 2, b + 1, 2))
print(evens)



