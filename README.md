numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15]
primes = []
not_primes = []
for i in numbers:
    for j in range(2, i):
        if i % j == 0:
            not_primes.append(i)
            break
    if i not in not_primes:
        primes.append(i)
primes.remove(1)
print(primes)
print(not_primes)
