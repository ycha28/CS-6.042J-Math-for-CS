**Problem 1**
**a)** $\exists$x$\in$X: $S(x)$$\wedge$$A(x)$
**b)** $\forall$x$\in$X: $T(x)$$\wedge$$S(x)$$\rightarrow$$A(x)$
**c)** $\neg$($\exists$x$\in$X: $T(x)$$\wedge$$\neg$$A(x)$)
**d)** $\exists$x,y,z$\in$X: ($\neg$$E(x,y)$$\wedge$$\neg$$E(z,y)$$\wedge$$\neg$$E(x,z)$) $T(x)$$\wedge$$\neg$$S(x)$$T(y)$$\wedge$$\neg$$S(y)$$T(z)$$\wedge$$\neg$$S(z)$

**Problem 2**
**a)**
| $P$ | $Q$ | $R$ | ($\neg$($P$$\vee$($Q$$\wedge$$R$)) | ($\neg$$P$)$\wedge$($\neg$$Q$$\vee$$\neg$$R$) |
|1| | T | T | T | F | F
|2| | T | T | F | F | F
|3| | T | F | T | F | F
|4| | T | F | F | F | F
|5| | F | T | T | F | F
|6| | F | T | F | T | T
|7| | F | F | T | T | T
|8| | F | F | F | T | T

The two sides of the implication agree in all cases, so they are equal.
**b)**
| $P$ | $Q$ | $R$ | ($\neg$($P$$\wedge$($Q$$\vee$$R$)) | ($\neg$$P$)$\vee$($\neg$$Q$$\vee$$\neg$$R$) |
|1| | T | T | T | F | F
|2| | T | T | F | F | T
|3| | T | F | T | F | T
|4| | T | F | F | T | T
|5| | F | T | T | T | T
|6| | F | T | F | T | T
|7| | F | F | T | T | T
|8| | F | F | F | T | T
The two sides of the implication do not agree in all cases, so they are not equal.

**Problem 3**
**a)** 
i) $A$ $\wedge$ $B$ = $\neg$($A$ nand $B$)
ii) $A$ $\vee$ $B$ = $\neg$$A$ nand $\neg$$B$
iii) $A$ $\rightarrow$ $B$ = $A$ nand $\neg$$B$

**b)**
(A nand A)

**c)**
True = ($A$ nand $A$) nand $A$
False = (($A$ nand $A$) nand $A$) nand (($A$ nand $A$) nand $A$)

**Problem 4**
1. Divide the 12 coins into three piles containing four coins each. Take two of the piles put them on each side of the balance
scale. If the two piles are perfectly balanced, then we know that they contain all real coins. Divide one of the piles by
four to obtain the weight of the real coin. If the two piles are not balanced, then we know that the heavier pile contains
all real coins. Divide that pile by four to obtain the weight of the real coin. Subtract three times the weight of the real
coin from the lighter pile; the remainder is the weight of the fake coin.
2. Take the lightest of the three piles and split it in half. Put two coins each on each side of the balance scale. The 
lighter side contains the fake coin.
3. Take the lighter side and put each coin on each side of the balance scale. The side that weighs less contains the fake 
coin.

**Problem 5**
If r^1/5 is rational, then r is rational.

Assume that r^1/5 is rational. Then there must be some quotient of integers m/n that equals r^1/5. If we multiply r^1/5 = m/n to the fifth power on both sides, then we get r = m^5/n^5. m^5 and n^5 must be integers, so r is also rational.

**Problem 6**
Case 1: If one of w, x, or y is odd, then the resulting sum w^2 + x^2 + y^2 must also be odd. This is because the square of an odd number is always odd, and the sum of two even numbers and an odd number is always odd. If the sum is odd, then z must also be odd, since the square root of an odd number can never be an even number.
Case 2: If all three variables w, x, and y are odd, then the resulting sum w^2 + x^2 + y^2 must also be odd. This is because the sum of three odd numbers is always odd. By the same reasoning described above, z must also be odd.
Case 3: If all three variables are even, then the resulting sum w^2 + x^2 + y^2 must also be even. Then the resulting z will be even if the sum adds up to an integer with an integer square root.
Case 4: If two of the variables are odd, then we have the following situation:

Let w = 2i, x = 2j + 1, and y = 2k + 1. Then the sum w^2 + x^2 + y^2 results in 

4i^2 + (4j^2 + 4j + 1) + (4k^2 + 4k + 1)
4i^2 + 4j^2 +4k^2 + 4j + 4k + 2
4(i^2 + j^2 + k^2 + j + k) + 2

This sum is not divisible by 4 because there is an extra 2 added at the end. However, we know that if z is an even integer,
then z^2 must be a multiple of 4. Since the value of z^2 is not a multiple of 4, z must be an odd integer.
