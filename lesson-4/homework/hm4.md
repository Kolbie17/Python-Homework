# Sort a Dictionary by Value

# Create a sample dictionary
scores = {"Alice": 88, "Bob": 95, "Charlie": 70, "David": 92}

# Sort by value in ascending order
ascending = dict(sorted(scores.items(), key=lambda item: item[1]))

# Sort by value in descending order
descending = dict(sorted(scores.items(), key=lambda item: item[1], reverse=True))

# Display results
print("Original dictionary:", scores)
print("Ascending order:", ascending)
print("Descending order:", descending)


# Add a Key to a Dictionary

# Original dictionary
my_dict = {0: 10, 1: 20}

# Add a new key and value
my_dict[2] = 30

# Display the updated dictionary
print("Updated dictionary:", my_dict)


# Concatenate Multiple Dictionaries

# Sample dictionaries
dic1 = {1: 10, 2: 20}
dic2 = {3: 30, 4: 40}
dic3 = {5: 50, 6: 60}

# Merge all dictionaries into one
result = {}
for d in (dic1, dic2, dic3):
    result.update(d)

# Display the result
print("Expected Result:\n", result)


# Generate a Dictionary with Squares

# Ask the user for a number
n = int(input("Enter a number: "))

# Generate the dictionary
squares = {x: x*x for x in range(1, n + 1)}

# Display the result
print("Sample Dictionary:", squares)


# Dictionary of Squares (1 to 15)

# Generate the dictionary
squares = {x: x*x for x in range(1, 16)}

# Display the result
print(squares)


# Create a Set

# Create a set of numbers
my_set = {1, 2, 3, 4, 5}

# Display the set
print("Created set:", my_set)


# Iterate Over a Set

# Create a set of fruits
fruits = {"apple", "banana", "cherry", "mango"}

# Iterate through the set
print("Fruits in the set:")
for fruit in fruits:
    print(fruit)


# Add Member(s) to a Set

# Create an initial set
my_set = {"apple", "banana", "cherry"}

# Add a single member
my_set.add("mango")

# Add multiple members
my_set.update(["orange", "grape"])

# Display the updated set
print("Updated set:", my_set)


# Remove Item(s) from a Set

# Create a sample set
my_set = {"apple", "banana", "cherry", "mango", "orange"}

# Remove a specific item using remove()
my_set.remove("banana")   # Raises error if item not found

# Safely remove an item using discard()
my_set.discard("grape")   # No error if item not found

# Remove and return a random item using pop()
removed_item = my_set.pop()

# Display the results
print("Set after removals:", my_set)
print("Randomly removed item:", removed_item)


# Remove an Item if Present in the Set

# Create a sample set
my_set = {"apple", "banana", "cherry"}

# Item to remove
item = "banana"

# Check and remove if present
if item in my_set:
    my_set.remove(item)
    print(f"'{item}' was removed from the set.")
else:
    print(f"'{item}' is not in the set.")

# Display the updated set
print("Updated set:", my_set)
