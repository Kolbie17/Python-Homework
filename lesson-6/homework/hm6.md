def modify_string(txt):
    vowels = 'aeiouAEIOU'

    def helper(s, i):
        if i + 3 >= len(s):
            return s  # базовый случай: меньше 3 символов — возвращаем как есть

        # позиция, где хотим вставить "_"
        pos = i + 3
        if s[pos - 1] in vowels or (pos < len(s) and s[pos] == '_'):
            pos += 1  # сдвигаем вперёд, если на 3-й позиции гласная или после уже стоит "_"

        if pos >= len(s):
            return s  # не вставляем "_" в конец

        s = s[:pos] + '_' + s[pos:]
        return helper(s, pos + 1)  # двигаемся дальше после вставленного "_"

    return helper(txt, 0)


n = int(input().strip())

for i in range(n):
    print(i ** 2)

i = 1
while i <= 10:
    print(i)
    i += 1


n = 5  # number of rows

i = 1
while i <= n:
    j = 1
    while j <= i:
        print(j, end=" ")
        j += 1
    print()  # переход на новую строку
    i += 1

num = int(input("Enter number: "))
i = 1
total = 0

while i <= num:
    total += i
    i += 1

print("Sum is:", total)


num = int(input("Enter a number: "))

i = 1
while i <= 10:
    print(num * i)
    i += 1
numbers = [12, 75, 150, 180, 145, 525, 50]

for num in numbers:
    if num > 500:
        break
    elif num > 150:
        continue
    elif num % 5 == 0:
        print(num)


num = int(input("Enter a number: "))
count = 0

while num > 0:
    num //= 10   # убираем последнюю цифру
    count += 1

print("Total digits:", count)

num = input("Enter a number: ")
print("Total digits:", len(num))


n = 5  # можно заменить на любое число

for i in range(n, 0, -1):
    for j in range(i, 0, -1):
        print(j, end=" ")
    print()  # переход на новую строку


n = 5
i = n

while i >= 1:
    j = i
    while j >= 1:
        print(j, end=" ")
        j -= 1
    print()
    i -= 1

list1 = [10, 20, 30, 40, 50]

for i in range(len(list1) - 1, -1, -1):
    print(list1[i])

list1 = [10, 20, 30, 40, 50]

i = len(list1) - 1
while i >= 0:
    print(list1[i])
    i -= 1


for i in range(-10, 0):
    print(i)


for i in range(5):
    print(i)
print("Done!")

start = int(input("Enter start of range: "))
end = int(input("Enter end of range: "))

print(f"Prime numbers between {start} and {end}:")

for num in range(start, end + 1):
    if num > 1:  # простые числа начинаются с 2
        for i in range(2, int(num ** 0.5) + 1):
            if num % i == 0:
                break
        else:
            print(num)


n = 10  # количество элементов
a, b = 0, 1

print("Fibonacci sequence:")

for i in range(n):
    print(a, end="  ")
    a, b = b, a + b


num = int(input("Enter a number: "))
factorial = 1

for i in range(1, num + 1):
    factorial *= i

print(f"{num}! = {factorial}")


def uncommon_elements(list1, list2):
    return [x for x in list1 if x not in list2] + [x for x in list2 if x not in list1]

