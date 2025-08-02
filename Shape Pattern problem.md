# ⭐ Pattern Programs in Python (35 Total)

This repository contains classic pattern printing problems in Python — great for beginners practicing nested loops and logic building.

---
1. Square Pattern
for i in range(5):
    for j in range(5):
        print("*", end="")
    print()

*****
*****
*****
*****
*****

2. Left-Aligned Triangle
for i in range(1, 6):
    print("*" * i)

*
**
***
****
*****

3. Inverted Left-Aligned Triangle
for i in range(5, 0, -1):
    print("*" * i)

*****
****
***
**
*

4. Number Triangle
for i in range(1, 6):
    for j in range(1, i + 1):
        print(j, end=" ")
    print()

1
1 2
1 2 3
1 2 3 4
1 2 3 4 5

5. Half Diamond
for i in range(1, 6):
    print("*" * i)
for i in range(4, 0, -1):
    print("*" * i)

*
**
***
****
*****
****
***
**
*

6. Right-Aligned Triangle
for i in range(1, 6):
    print(" " * (5 - i) + "*" * i)

    *
   **
  ***
 ****
*****

7. Inverted Right-Aligned Triangle
for i in range(5, 0, -1):
    print(" " * (5 - i) + "*" * i)

*****
 ****
  ***
   **
    *

8. Pyramid
for i in range(1, 6):
    print(" " * (5 - i) + "*" * (2 * i - 1))

    *
   ***
  *****
 *******
*********

9. Inverted Pyramid
for i in range(5, 0, -1):
    print(" " * (5 - i) + "*" * (2 * i - 1))

*********
 *******
  *****
   ***
    *

10. Centered Triangle
for i in range(1, 6):
    print(" " * (5 - i) + "* " * i)

    * 
   * * 
  * * * 
 * * * * 
* * * * * 

11. Inverted Centered Triangle
for i in range(5, 0, -1):
    print(" " * (5 - i) + "* " * i)

* * * * * 
 * * * * 
  * * * 
   * * 
    * 

12. Full Diamond
for i in range(1, 6):
    print(" " * (5 - i) + "* " * i)
for i in range(4, 0, -1):
    print(" " * (5 - i) + "* " * i)

    * 
   * * 
  * * * 
 * * * * 
* * * * * 
 * * * * 
  * * * 
   * * 
    * 

13. Hollow Pyramid
for i in range(1, 6):
    print(" " * (5 - i), end="")
    for j in range(1, i + 1):
        if j == 1 or j == i or i == 5:
            print("*", end="")
        else:
            print(" ", end="")
    print()

    *
   **
  * *
 *  *
*****

14. Inverted Hollow Triangle
for i in range(5):
    print(" " * i, end="")
    for j in range(5 - i):
        if j == 0 or j == 5 - i - 1 or i == 0:
            print("*", end="")
        else:
            print(" ", end="")
    print()

*****
*  *
* *
**
*

15. Hollow Diamond
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

    *
   * *
  *   *
 *     *
*       *
 *     *
  *   *
   * *
    *

16. Number Square
for i in range(1, 6):
    for j in range(1, 6):
        print(j, end=" ")
    print()

1 2 3 4 5 
1 2 3 4 5 
1 2 3 4 5 
1 2 3 4 5 
1 2 3 4 5 

17. Number Pyramid
for i in range(1, 6):
    print(" " * (5 - i) + (str(i) + " ") * i)

    1 
   2 2 
  3 3 3 
 4 4 4 4 
5 5 5 5 5 

18. Continuous Numbers
num = 1
for i in range(1, 6):
    for j in range(i):
        print(num, end=" ")
        num += 1
    print()

1 
2 3 
4 5 6 
7 8 9 10 
11 12 13 14 15 

19. Reverse Number Triangle
for i in range(5, 0, -1):
    for j in range(1, i + 1):
        print(j, end=" ")
    print()

1 2 3 4 5 
1 2 3 4 
1 2 3 
1 2 
1 

20. Right-Aligned Number Triangle
for i in range(1, 6):
    print(" " * (5 - i), end="")
    for j in range(1, i + 1):
        print(j, end="")
    print()

    1
   12
  123
 1234
12345

21. Alphabet Triangle
for i in range(1, 6):
    for j in range(i):
        print(chr(65 + j), end=" ")
    print()

A 
A B 
A B C 
A B C D 
A B C D E 

22. Reverse Alphabet Triangle
for i in range(5, 0, -1):
    for j in range(i):
        print(chr(65 + j), end=" ")
    print()

A B C D E 
A B C D 
A B C 
A B 
A 

23. Alphabet Pyramid
for i in range(1, 6):
    print(" " * (5 - i) + (chr(65 + i - 1) + " ") * i)

    A 
   B B 
  C C C 
 D D D D 
E E E E E 

24. Continuous Alphabet
ch = 65
for i in range(1, 6):
    for j in range(i):
        print(chr(ch), end=" ")
        ch += 1
    print()

A 
B C 
D E F 
G H I J 
K L M N O 

25. Hollow Square
for i in range(5):
    for j in range(5):
        if i == 0 or i == 4 or j == 0 or j == 4:
            print("*", end="")
        else:
            print(" ", end="")
    print()

*****
*   *
*   *
*   *
*****

26. X Pattern
for i in range(5):
    for j in range(5):
        if i == j or i + j == 4:
            print("*", end="")
        else:
            print(" ", end="")
    print()

*   *
 * * 
  *  
 * * 
*   *

27. Plus Pattern
for i in range(5):
    for j in range(5):
        if i == 2 or j == 2:
            print("*", end="")
        else:
            print(" ", end="")
    print()

  *  
  *  
*****
  *  
  *  

28. Left Arrow
for i in range(5):
    for j in range(5):
        if j == 0 or (i == 2 and j <= 3):
            print("*", end="")
        else:
            print(" ", end="")
    print()

*    
*    
**** 
*    
*    

29. Right Arrow
for i in range(5):
    for j in range(5):
        if j == 4 or (i == 2 and j >= 1):
            print("*", end="")
        else:
            print(" ", end="")
    print()

    *
    *
 ****
    *
    *

30. Sandglass Star
for i in range(5, 0, -1):
    print(" " * (5 - i) + "* " * i)
for i in range(2, 6):
    print(" " * (5 - i) + "* " * i)

* * * * * 
 * * * * 
  * * * 
   * * 
    * 
   * * 
  * * * 
 * * * * 
* * * * * 

31. Hourglass Star
for i in range(5):
    print(" " * i + "*" * (9 - 2 * i))
for i in range(1, 5):
    print(" " * (4 - i) + "*" * (2 * i + 1))

*********
 *******
  *****
   ***
    *
   ***
  *****
 *******
*********

32. Pascal’s Triangle
from math import comb
for i in range(5):
    for j in range(5 - i):
        print(" ", end="")
    for j in range(i + 1):
        print(comb(i, j), end=" ")
    print()

     1 
    1 1 
   1 2 1 
  1 3 3 1 
 1 4 6 4 1 

33. Binary Triangle
for i in range(1, 6):
    for j in range(1, i + 1):
        print((i + j) % 2, end=" ")
    print()

0 
1 0 
0 1 0 
1 0 1 0 
0 1 0 1 0 

34. Floyd’s Triangle
num = 1
for i in range(1, 6):
    for j in range(i):
        print(num, end=" ")
        num += 1
    print()

1 
2 3 
4 5 6 
7 8 9 10 
11 12 13 14 15 

35. Butterfly Pattern
n = 5
for i in range(1, n + 1):
    print("*" * i + " " * (2 * (n - i)) + "*" * i)
for i in range(n, 0, -1):
    print("*" * i + " " * (2 * (n - i)) + "*" * i)

*        *
**      **
***    ***
****  ****
**********
**********
****  ****
***    ***
**      **
*        *


