**Problem 1**

**a)**
If a1 < a2, then a3 must be smaller than a1. Consider the following situations where a3 > a1:

a1 < a2 < a3. This creates a 3-chain of monotonically increasing integers from a1 to a3.
a1 < a3 < a2 < a4. This creates a 3-chain of monotonically increasing integers from a1 to a2 to a4.
a4 < a1 < a3 < a2. This creates a 3-chain of monotonically decreasing integers from a2 to a3 to a4.

Therefore, a3 must be smaller than a1, which means the correct sequence is a3 < a1 < a2.

**b)**
The only place a4 can be is between a3 and a2, where a4 is less than a3 but greater than a2. Consider
the following situations:

a4 < a3 < a1 < a2. This creates a 3-chain of monotonically decreasing integers from a2 to a3 to a4.
a3 < a1 < a2 < a4. This creates a 3-chain of monotonically increasing integers from a1 to a2 to a4.
a3 < a4 < a1 < a2. No 3-chain sequence.
a3 < a1 < a4 <a2. No 3-chain sequence.

Therefore, a3 < a4 < a2 is the only valid sequence at this time.

**c)**
Placing any value of a5 anywhere will create a 3-chain. Consider the following situations:

a3 < a4 < a1 < a2 < a5. This creates a a3 < a4 < a5 3-chain.
a5 < a3 < a4 < a1 < a2. This creates a a5 < a4 < a1 3-chain (or a a5 < a4 < a2 3-chain).
a3 < a1 < a4 <a2 < a5. This creates a a3 < a4 < a5 3-chain.
a5 < a3 < a1 < a4 <a2. This creates a a5 < a4 < a2 3-chain (or a a5 < a3 < a1 3-chain).

If a5 < a4, then we will see a a3 < a4 < a5 3-chain. If a5 > a4, then we will see a a5 < a4 < a2 3-chain. Either way,
a 3 -chain is inevitable.

**d)**
Proof by contradiction. Assume that there is some sequence of five distinct integers where a 3-chain is not present.

From the previous parts, we proved that any sequence where a1 < a2 causes the insertion of a5 to result in a 3-chain. Now
we must consider the other case, where a1 > a2.

a1 > a2
a3 > a1 > a2 (a3 must be greater than a1, or else the insertion of a4 will result in a 3-chain)
a3 > a4 > a1 > a2 OR a3 > a1 > a4 > a2 (all other sequences contain 3-chains)

At this point, we encounter the same situation as above; the insertion of a5 at any point will result in a 3-chain.

Thus, regardless of whether we use a sequence where a1 > a2 or a2 > a1, the insertion of a5 will always result in a 3-chain.
This contradicts our original assumption, which means that any sequence of five distinct integers must contain a 3-chain.

**Problem 2**
Proof by induction.

Let P(n) = for all integers from 0 to n, i^3 = ((n (n + 1))/2)^2.

Base case: 
When n = 0, i^3 = ((0 (0 + 1))/2)^2
                = (0)^2
                = 0
                
0^3 = 0, so the base case is valid.

Inductive step:
Given that P(n) is true, we know the following:

0^3 + 1^3 + ... n^3 = ((n (n + 1))/2)^2

If we add (n + 1)^3 to both sides, we get:
0^3 + 1^3 + ... n^3 + (n + 1)^3 = (n^2 + n)^2/4 + (n + 1)^2 * (n + 1)
                                = (n^2 * (n + 1)^2)/4 + (n + 1)^2 * (n + 1)
                                = (n + 1)^2 * (n^2 + 4n + 4) / 4
                                = ((n + 1)^2 * (n + 2)^2) / 4
                                = ((n + 1) * (n + 2)) / 2)^2

Thus, P(n + 1) is true, which means that P(n) implies P(n + 1). Therefore, P(n) is true for all nonnegative integers
by induction.



