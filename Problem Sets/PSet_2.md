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

**Problem 3**
If we define p as the perimeter of infected students (i.e., the number of edges with an X on only one side), then we can find that p never increases with each time-step. We prove this by induction.

Let I be the perimeter of the initial set of infected students. For all n >= 0 where n represents the number of time-steps, let P(n) = p(n) < I.

Base case: 
When n = 0, p(n) = 0. Since 0 < I, the base case holds true.

Inductive step:
Assume that P(n) is true. When we increment the time-step, we know that a new student becomes infected via one of two methods:

1. The newly infected is adjacent to two infected students. In this case, the perimeter remains the same, because the 
new square removes two edges from the perimeter but adds two edges of its own.
2. The newly infected is adjacent to three infected students. In this case, the perimeter decreases, because the
new square removes three edges from the perimeter while adding only one edge of its own.

Thus, with the n + 1 step, we know that the total perimeter can only decrease, not increase. Since the perimeter can only decrease, p(n) < I, so our initial proposition holds true. Therefore, by induction, we can conclude that the perimeter
never increases from its initial set.

If the perimeter of the set of students who are completely infected (i.e., every square is marked X) is greater than the 
initial perimeter I, then we know that no matter how many time-steps pass, not all of the students will become infected.
This follows from the previous proof, which showed that the final perimeter can never increase beyond I. The set of 
total infection has a perimeter of 4n, where n is the length of each side of the square. Since each square has a perimeter
of 4, at least n squares must be infected for the whole grid to be infected.

**Problem 4**
This proof does not work because the inductive step makes an extra assumption, namely that n >= 1. If n < 1, then the denominator would fail to return a known value (we do not know what a^-1 equals in this instance). That is, we need to prove that P(n) is true for all n >= 1, not just P(n). We need to prove this in order to show that a^(n - 1) = 1, as the author assumes in the inductive step. However, this hypothesis falls apart when n = 1, as a^n does not necessarily equal 1. Therefore, the proof is invalid.

**Problem 5**
Proof by strong induction.

Let P(n) = for all n E N, G(n) = 3^n - 2^n. 

Base cases: G(0) = 0 = 3^0 - 2^0
                   0 = 1 - 1
                   0 = 0
            G(1) = 1 = 3^1 - 2^1
                   1 = 3 - 2
                   1 = 1
                   
The base cases for 0 and 1 both hold.

Inductive step:
G(n + 1) = 5(G(n)) - 6(G(n - 1))
         = 5(3^n - 2^n) - 6(3^(n - 1) - 2^(n -1))
         = 5(3^n - 2^n) - 2(3^n) - 3(2^n)
         = 3^n(5 - 2) - 2^n(5 - 3)
         = 3^n(3) - 2^n(2)
         = 3^(n + 1) - 2^(n + 1)

Thus, P(n + 1) holds, and therefore P(n) is true for all values of n.

**Problem 6**
**a)** 
Proposition: a row move cannot change the order of the board.
Proof: A row move can only change a tile to an adjacent cell. If it moves the tile to the right, the tile's position increases by 1, but the order remains the same, and if it moves a tile to the left, the tile's position decreases by 1, but the order still remains the same. Therefore, the order of the board cannot be changed by a row move.

**b)**
Proposition: 3 pairs of tiles will have their order changed by a column move.
Proof: When a letter gets moved down, the three letters that originally came after the letter experience a change in relative
order. Therefore, the relative order between the moved letter and each of the three letters changes. A move up will have the
same effect; the pairs of the moved letter and each of the three letters will experience a change in relative order.

**c)**
Proposition: a row move has no effect on the number of inversions.
Proof: Earlier we proved that a row move cannot change the order of a board. Therefore, it can have no effect on the number
of inversions, as the number of inversions can only be changed by a change in the order of the board. 

**d)**
Proposition: a column move will change the parity of the board.
Proof: A column move can change the order of the board and therefore add or remove inversions. Consider the following cases:
1. Three inversions with the letter to be moved existed before the move. After the move, all three inversions are corrected.
This reduces the total number of inversions by three and changes the parity of the board.
2. No inversions involving the letter to be moved existed before the move. After the move, three new inversions are introduced, changing the parity.
3. One inversion existed before the move. After the move, two new inversions are introduced and the original inversion is removed; this results in a net of one new inversion, changing the parity.
4. Two inversions existed before the move. After the move, one inversion is introduced and two are removed. This results
in a net of a negative inversion, changing the parity.

**e)**
Proposition: The parity of the number of inversions is different from the parity of the row containing the blank square.
Proof: 
Consider the following cases:
1. A row move is made. In this case, the parity of the row containing the blank tile and the parity of the number of inversions remain the same, as a row move does not affect the parity of anything. That is, the parity of the number of inversions will continue to be odd, and the parity of the row containing the blank space will still be even.
2. A column move is made. In this case, the parity of the number of inversions flips from odd to even or vice versa. However, the parity of the row with the blank tile flips to the opposite value as well, as the blank tile now exists in an adjacent row. So the parity of the total number of inversions is still different from the parity of the row containing the blank tile.

Therefore, the parity of the number of inversions will always be different from the parity of the row containing the blank square.

**f)**
If the parity of the number of inversions is always different from the parity of the row containing the blank square, then the correct configuration of the board can never be achieved, since that configuration contains zero inversions (i.e., an even number of inversions) and the blank tile is in row 4 (i.e., the row containing the blank tile has an even parity).

**Problem 7**
Proposition: The number of Z-lings will at most be twice the number of B-lings.
Proof: Proof by strong induction.

Let P(n) be the proposition that the number of B-lings will never be less than the number of Z-lings. That is, 
P(n) : b(n) <= z(n) for all n E N

Base case: 
P(0) : b(0) <= z(0)
At step 0, we know that there are 200 Z-lings and 800 B-lings. 200 <= 800, so the base case holds.

Inductive step:
We assume that P(0), P(1), P(2) ... P(n) is true because of strong induction. At P(n + 1), the following must also be true:

1. Before the reproduction occurs, the number of B-lings is greater than the current number of Z-lings. This is true because
of P(n).
2. The total number of Z-lings is equal to z(n) + z(n)/2 + ((b(n) - z(n))/2. This simplifies to z(n) + b(n)/2.
3. The total number of B-lings is equal to b(n) + z(n)/2 + 2((b(n) - z(n))/2. This simplifies to 2b(n) + z(n)/2.

Given that b(n) >= z(n), we can conclude that z(n) will never be greater than b(n), as 2b(n) + z(n)/2 will always be greater than z(n) + b(n)/2. Therefore, by the inductive step, we conclude that the number of B-lings will always be greater than or equal to the number of Z-lings. It naturally follows that the weaker hypothesis (i.e., the number of Z-lings will always be at least twice as great as the number of B-lings) is also true.
