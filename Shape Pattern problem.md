# ⭐ Pattern Programs in Python (35 Total)

This repository contains classic pattern printing problems in Python — great for beginners practicing nested loops and logic building.

---

## 🔹 1. Solid Square
```python
for i in range(5):
    for j in range(5):
        print("*", end="")
    print()
🔹 2. Left-Aligned Triangle

for i in range(1, 6):
    print("*" * i)
🔹 3. Inverted Left-Aligned Triangle

for i in range(5, 0, -1):
    print("*" * i)
🔹 4. Number Triangle
for i in range(1, 6):
    for j in range(1, i + 1):
        print(j, end=" ")
    print()
🔹 5. Half Diamond

for i in range(1, 6):
    print("*" * i)
for i in range(4, 0, -1):
    print("*" * i)
🔹 6. Right-Aligned Triangle

for i in range(1, 6):
    print(" " * (5 - i) + "*" * i)
🔹 7. Inverted Right-Aligned Triangle

for i in range(5, 0, -1):
    print(" " * (5 - i) + "*" * i)
🔹 8. Pyramid

for i in range(1, 6):
    print(" " * (5 - i) + "*" * (2 * i - 1))
🔹 9. Inverted Pyramid

for i in range(5, 0, -1):
    print(" " * (5 - i) + "*" * (2 * i - 1))
🔹 10. Centered Triangle

for i in range(1, 6):
    print(" " * (5 - i) + "* " * i)
🔹 11. Inverted Centered Triangle

for i in range(5, 0, -1):
    print(" " * (5 - i) + "* " * i)
🔹 12. Full Diamond

for i in range(5, 0, -1):
    print(" " * (5 - i) + "* " * i)
for i in range(2, 6):
    print(" " * (5 - i) + "* " * i)
🔹 13. Hollow Pyramid

for i in range(1, 6):
    print(" " * (5 - i), end="")
    for j in range(1, i + 1):
        if j == 1 or j == i or i == 5:
            print("*", end="")
        else:
            print(" ", end="")
    print()
🔹 14. Inverted Hollow Triangle

for i in range(5):
    print(" " * i, end="")
    for j in range(5 - i):
        if j == 0 or j == 5 - i - 1 or i == 0:
            print("*", end="")
        else:
            print(" ", end="")
    print()
🔹 15. Hollow Diamond

for i in range(1, 6):
    print(" " * (5 - i), end="")
    print("*", end="")
    if i != 1:
        print(" " * (2 * i - 3), end="*")
    print()
for i in range(4, 0, -1):
    print(" " * (5 - i), end="")
    print("*", end="")
    if i != 1:
        print(" " * (2 * i - 3), end="*")
    print()
🔹 16. Pascal's Triangle

n = 5
for i in range(n):
    print("  " * (n - i - 1), end="")
    num = 1
    for j in range(i + 1):
        print(f"{num}   ", end="")
        num = num * (i - j) // (j + 1)
    print()
🔹 17. Number Pyramid
for i in range(1, 5):
    print(" " * (4 - i), end="")
    for j in range(i, 0, -1):
        print(j, end="")
    for j in range(2, i + 1):
        print(j, end="")
    print()
for i in range(3, 0, -1):
    print(" " * (4 - i), end="")
    for j in range(i, 0, -1):
        print(j, end="")
    for j in range(2, i + 1):
        print(j, end="")
    print()
🔹 18. Double Arrow
for i in range(1, 6):
    print("*" * (6 - i) + " " * (2 * (i - 1)) + "*" * (6 - i))
for i in range(5, 0, -1):
    print("*" * (6 - i) + " " * (2 * (i - 1)) + "*" * (6 - i))
🔹 19. Butterfly
for i in range(1, 6):
    print("*" * i + " " * (10 - 2 * i) + "*" * i)
for i in range(4, 0, -1):
    print("*" * i + " " * (10 - 2 * i) + "*" * i)
🔹 20. Hollow Rectangle

for i in range(1, 6):
    for j in range(1, 5):
        if i == 1 or i == 5 or j == 1 or j == 4:
            print("*", end="")
        else:
            print(" ", end="")
    print()
🔹 21. Number Count Triangle
cnt = 1
for i in range(1, 6):
    for j in range(1, i + 1):
        print(cnt, end=" ")
        cnt += 1
    print()
🔹 22. Binary Triangle

for i in range(1, 6):
    for j in range(1, i + 1):
        print((i + j) % 2, end=" ")
    print()
🔹 23. Centered Star Triangle

for i in range(3):
    print("  " * (2 - i) + "*   " * (i + 1))
🔹 24. Hourglass Pattern

for i in range(1, 6):
    print("*" * i + " " * (2 * (5 - i)) + "*" * i)
for i in range(4, 0, -1):
    print("*" * i + " " * (2 * (5 - i)) + "*" * i)
🔹 25. Hollow Centered Triangle

for i in range(1, 6):
    print(" " * (5 - i), end="")
    for j in range(1, i + 1):
        if i == 1 or i == 5 or j == 1 or j == i:
            print("*", end="")
        else:
            print(" ", end="")
    print()
🔹 26. Reverse Number Triangle
for i in range(1, 7):
    print((str(i) + " ") * (7 - i))
🔹 27. Snake Number Pattern
val = 1
for i in range(1, 5):
    print("  " * (i - 1), end="")
    for j in range(5 - i + 1):
        print(val, end=" ")
        val += 1
    for j in range(5 - i):
        print(val, end=" ")
        val += 1
    print()
🔹 28. Full Diamond Using *
for i in range(1, 6):
    print(" " * (5 - i) + "* " * i)
for i in range(4, 0, -1):
    print(" " * (5 - i) + "* " * i)
🔹 29. Same as 19 (Butterfly)
🔹 30. Number Palindrome Pyramid

for i in range(1, 6):
    print(" " * (5 - i), end="")
    for j in range(i, 0, -1):
        print(j, end=" ")
    for j in range(2, i + 1):
        print(j, end=" ")
    print()
🔹 31. Concentric Number Square

for i in range(1, 8):
    for j in range(1, 8):
        min_val = min(i, j, 8 - i, 8 - j)
        print(5 - min_val + 1, end=" ")
    print()
🔹 32. Alphabet Incremental

for i in range(ord('E'), ord('A') - 1, -1):
    for j in range(i, ord('E') + 1):
        print(chr(j), end=" ")
    print()
🔹 33. Alternate Case Characters

ch = ord('a')
for i in range(1, 6):
    for j in range(1, i + 1):
        if (i + j) % 2 == 0:
            print(chr(ch).upper(), end=" ")
        else:
            print(chr(ch), end=" ")
        ch += 1
    print()
🔹 34. Reverse Alphabet

for i in range(ord('E'), ord('A') - 1, -1):
    for j in range(i, ord('A') - 1, -1):
        print(chr(j), end=" ")
    print()
🔹 35. Palindromic Number Pyramid
for i in range(1, 5):
    for j in range(1, i + 1):
        print(j, end="")
    print(" " * (2 * (4 - i)), end="")
    for j in range(i, 0, -1):
        print(j, end="")
    print()
