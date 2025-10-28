# Age Calculator

# Ask for user's name and year of birth
name = input("Enter your name: ")
year_of_birth = int(input("Enter your year of birth: "))

# Get the current year
from datetime import date
current_year = date.today().year

# Calculate age
age = current_year - year_of_birth

# Display result
print(f"Hello, {name}! You are {age} years old in {current_year}.")


# Extract specific car names from text

txt = 'LMaasleitbtui'

# Target car names
cars = ['Lacetti', 'Malibu']

# Extract by checking if all letters of the car name appear in order (not necessarily consecutive)
def contains_in_order(word, text):
    it = iter(text.lower())
    return all(char.lower() in it for char in word.lower())

found_cars = [car for car in cars if contains_in_order(car, txt)]

print("Extracted car names:", found_cars)


# Extract car names from text
txt = 'MsaatmiazD'

# Target car names
cars = ['Mazda', 'Matiz', 'Lacetti', 'Malibu']

# Function to check if all letters of the car name appear in order (not necessarily consecutively)
def contains_in_order(word, text):
    it = iter(text.lower())
    return all(char.lower() in it for char in word.lower())

# Find which car names are hidden in the text
found_cars = [car for car in cars if contains_in_order(car, txt)]

print("Extracted car names:", found_cars)


# Extract residence area from text

import re

txt = "I'am John. I am from London"

# Use regular expression to find the word after "from"
match = re.search(r'\bfrom\s+([A-Za-z]+)', txt)

if match:
    area = match.group(1)
    print("Residence area:", area)
else:
    print("No residence area found.")


# Reverse String Program

# Ask the user for input
text = input("Enter a string: ")

# Reverse the string using slicing
reversed_text = text[::-1]

# Display the result
print("Reversed string:", reversed_text)


# Count Vowels in a String

# Ask the user for input
text = input("Enter a string: ")

# Define vowels
vowels = "aeiouAEIOU"

# Count vowels
count = sum(1 for char in text if char in vowels)

# Display the result
print("Number of vowels:", count)

# Find Maximum Value

# Ask the user for a list of numbers
numbers = input("Enter numbers separated by spaces: ")

# Convert the input string to a list of numbers
numbers_list = [float(num) for num in numbers.split()]

# Find the maximum value
max_value = max(numbers_list)

# Display the result
print("The maximum value is:", max_value)


# Check Palindrome

# Ask the user for input
word = input("Enter a word: ")

# Convert to lowercase for consistency
word = word.lower()

# Check if it reads the same forward and backward
if word == word[::-1]:
    print("Yes, it's a palindrome!")
else:
    print("No, it's not a palindrome.")

# Extract Email Domain

# Ask the user for an email address
email = input("Enter your email address: ")

# Split the email at '@' and take the second part (domain)
if "@" in email:
    domain = email.split('@')[1]
    print("Email domain:", domain)
else:
    print("Invalid email address.")

# Generate Random Password

import random
import string

# Ask user for desired password length
length = int(input("Enter the desired password length: "))

# Combine letters, digits, and special characters
characters = string.ascii_letters + string.digits + string.punctuation

# Generate random password
password = ''.join(random.choice(characters) for _ in range(length))

# Display the result
print("Your random password is:", password)




