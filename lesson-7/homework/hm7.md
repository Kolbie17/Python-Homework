def is_prime(n):
    if n <= 1:
        return False  # 1 va manfiy sonlar tub emas
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            return False  # Agar bo‘linadigan topilsa, tub emas
    return True  # Aks holda, tub son


print(is_prime(4))  # False
print(is_prime(7))  # True
print(is_prime(1))  # False
print(is_prime(13)) # True
print(is_prime(15)) # False

def digit_sum(k):
    return sum(int(digit) for digit in str(k))


print(digit_sum(24))   # 6  (2 + 4)
print(digit_sum(502))  # 7  (5 + 0 + 2)
print(digit_sum(1234)) # 10 (1 + 2 + 3 + 4)


def digit_sum(k):
    total = 0
    while k > 0:
        total += k % 10   # oxirgi raqamni qo‘shamiz
        k //= 10          # oxirgi raqamni olib tashlaymiz
    return total

print(digit_sum(24))   # 6
print(digit_sum(502))  # 7

def powers_of_two(N):
    k = 1
    power = 2 ** k
    while power <= N:
        print(power, end=" ")
        k += 1
        power = 2 ** k
powers_of_two(10)



def powers_of_two(N):
    for k in range(1, N):
        if 2 ** k <= N:
            print(2 ** k, end=" ")
        else:
            break
powers_of_two(50)
