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
