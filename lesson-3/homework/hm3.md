# Create and Access List Elements

# Create a list of fruits
fruits = ["Apple", "Banana", "Cherry", "Mango", "Orange"]

# Print the third fruit (index 2 because indexing starts from 0)
print("The third fruit is:", fruits[2])


# Concatenate Two Lists

# Create two lists
list1 = [1, 2, 3, 4, 5]
list2 = [6, 7, 8, 9, 10]

# Concatenate the two lists
combined_list = list1 + list2

# Display the result
print("Concatenated list:", combined_list)

# Extract Elements from a List

# Given list of numbers
numbers = [10, 20, 30, 40, 50, 60, 70]

# Find the middle index
middle_index = len(numbers) // 2

# Extract first, middle, and last elements
extracted = [numbers[0], numbers[middle_index], numbers[-1]]


# Convert List to Tuple

# Create a list of favorite movies
movies = ["Inception", "Interstellar", "The Dark Knight", "Avatar", "Titanic"]

# Convert the list to a tuple
movies_tuple = tuple(movies)

# Display the result
print("Movies list:", movies)
print("Movies tuple:", movies_tuple)

# Display the result
print("Extracted elements:", extracted)



# Check Element in a List

# Create a list of cities
cities = ["New York", "London", "Paris", "Tokyo", "Dubai"]

# Check if "Paris" is in the list
if "Paris" in cities:
    print("Yes, Paris is in the list.")
else:
    print("No, Paris is not in the list.")


# Duplicate a List Without Using Loops

# Create a list of numbers
numbers = [1, 2, 3, 4, 5]

# Duplicate the list using multiplication
duplicated_list = numbers * 2

# Display the result
print("Original list:", numbers)
print("Duplicated list:", duplicated_list)


# Swap First and Last Elements of a List

# Given list of numbers
numbers = [10, 20, 30, 40, 50]

# Swap the first and last elements
numbers[0], numbers[-1] = numbers[-1], numbers[0]

# Display the result
print("List after swapping:", numbers)


# Slice a Tuple

# Create a tuple of numbers from 1 to 10
numbers = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10)

# Slice from index 3 to 7 (index 7 is excluded)
slice_part = numbers[3:7]

# Display the result
print("Sliced tuple:", slice_part)


# Count Occurrences in a List

# Create a list of colors
colors = ["red", "blue", "green", "blue", "yellow", "blue"]

# Count how many times "blue" appears
count_blue = colors.count("blue")

# Display the result
print("The color 'blue' appears", count_blue, "times in the list.")


# Find the Index of an Element in a Tuple

# Create a tuple of animals
animals = ("tiger", "elephant", "lion", "zebra", "giraffe")

# Find the index of "lion"
index_lion = animals.index("lion")

# Display the result
print("The index of 'lion' is:", index_lion)

# Merge Two Tuples

# Create two tuples
tuple1 = (1, 2, 3, 4, 5)
tuple2 = (6, 7, 8, 9, 10)

# Merge the tuples
merged_tuple = tuple1 + tuple2

# Display t


# Find the Length of a List and Tuple

# Create a list and a tuple
fruits = ["apple", "banana", "cherry", "mango"]
numbers = (10, 20, 30, 40, 50, 60)

# Find lengths using len()
list_length = len(fruits)
tuple_length = len(numbers)

# Display the results
print("Length of the list:", list_length)
print("Length of the tuple:", tuple_length)

# Convert Tuple to List

# Create a tuple of five numbers
numbers_tuple = (10, 20, 30, 40, 50)

# Convert the tuple to a list
numbers_list = list(numbers_tuple)

# Display the result
print("Tuple:", numbers_tuple)
print("List:", numbers_list)


# Find Maximum and Minimum in a Tuple

# Create a tuple of numbers
numbers = (15, 42, 7, 89, 23, 56)

# Find maximum and minimum values
max_value = max(numbers)
min_value = min(numbers)

# Display the results
print("Maximum value:", max_value)
print("Minimum value:", min_value)


# Reverse a Tuple

# Create a tuple of words
words = ("Python", "is", "fun", "to", "learn")

# Reverse the tuple using slicing
reversed_tuple = words[::-1]

# Display the result
print("Original tuple:", words)
print("Reversed tuple:", reversed_tuple)
