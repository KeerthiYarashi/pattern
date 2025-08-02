# ⭐ Pattern Programs in Python (35 Total)

This repository contains classic pattern printing problems in Python — great for beginners practicing nested loops and logic building.

---
# 1. Square Pattern
for i in range(5):
    for j in range(5):
        print("*", end="")
    print()
# Output:
# *****
# *****
# *****
# *****
# *****

# 2. Left-Aligned Triangle
for i in range(1, 6):
    print("*" * i)
# Output:
# *
# **
# ***
# ****
# *****

# 3. Inverted Left-Aligned Triangle
for i in range(5, 0, -1):
    print("*" * i)
# Output:
# *****
# ****
# ***
# **
# *

# 4. Number Triangle
for i in range(1, 6):
    for j in range(1, i + 1):
        print(j, end=" ")
    print()
# Output:
# 1
# 1 2
# 1 2 3
# 1 2 3 4
# 1 2 3 4 5

# 5. Half Diamond
for i in range(1, 6):
    print("*" * i)
for i in range(4, 0, -1):
    print("*" * i)
# Output:
# *
# **
# ***
# ****
# *****
# ****
# ***
# **
# *

# 6. Right-Aligned Triangle
for i in range(1, 6):
    print(" " * (5 - i) + "*" * i)
# Output:
#     *
#    **
#   ***
#  ****
# *****

# 7. Inverted Right-Aligned Triangle
for i in range(5, 0, -1):
    print(" " * (5 - i) + "*" * i)
# Output:
# *****
#  ****
#   ***
#    **
#     *

# 8. Pyramid
for i in range(1, 6):
    print(" " * (5 - i) + "*" * (2 * i - 1))
# Output:
#     *
#    ***
#   *****
#  *******
# *********

# 9. Inverted Pyramid
for i in range(5, 0, -1):
    print(" " * (5 - i) + "*" * (2 * i - 1))
# Output:
# *********
#  *******
#   *****
#    ***
#     *

# 10. Centered Triangle
for i in range(1, 6):
    print(" " * (5 - i) + "* " * i)
# Output:
#     *
#    * *
#   * * *
#  * * * *
# * * * * *

# 11. Inverted Centered Triangle
for i in range(5, 0, -1):
    print(" " * (5 - i) + "* " * i)
# Output:
# * * * * *
#  * * * *
#   * * *
#    * *
#     *

# 12. Full Diamond
for i in range(1, 6):
    print(" " * (5 - i) + "* " * i)
for i in range(4, 0, -1):
    print(" " * (5 - i) + "* " * i)
# Output:
#     *
#    * *
#   * * *
#  * * * *
# * * * * *
#  * * * *
#   * * *
#    * *
#     *

# 13. Hollow Pyramid
for i in range(1, 6):
    print(" " * (5 - i), end="")
    for j in range(1, i + 1):
        if j == 1 or j == i or i == 5:
            print("*", end="")
        else:
            print(" ", end="")
    print()
# Output:
#     *
#    **
#   * *
#  *  *
# *****

# 14. Inverted Hollow Triangle
for i in range(5):
    print(" " * i, end="")
    for j in range(5 - i):
        if j == 0 or j == 5 - i - 1 or i == 0:
            print("*", end="")
        else:
            print(" ", end="")
    print()
# Output:
# *****
# *  *
# * *
# **
# *

# 15. Hollow Diamond
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
# Output:
#     *
#    * *
#   *   *
#  *     *
# *       *
#  *     *
#   *   *
#    * *
#     *

# Output for remaining patterns will be appended...

