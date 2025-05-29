<p>Vishnu is very fond of Rummy. Rummy is a game played with standard set of cards. Each deck has 52 cards, 4 suits with 13 ranks each. In Rummy, however, multiple decks can be used in a single game. In our problem we ignore card suits and are only looking at ranks. Those are as follows (from lowest to highest): A, 2, 3, ..., 10, J, Q, K, (A). Ace is a special card that can be treated both as lowest (before 2) and highest rank (after K).</p>

<p>Rummy has different variants, our is as follows. Each player has a hand of exactly 13 cards. Cards are being discarded from a hand by constructing sets. Each card can belong to at most one set. There are two types of valid sets: <br>
<b>(1)</b> Exactly three cards of the same rank, for example (2, 2, 2) or (Q, Q, Q).<br>
<b>(2)</b> Sequence of at least three cards.</p>

<p> Sequence is a set of consecutive ranked cards, with at most one card for each rank. Some examples: (2, 3, 4, 5), (Q, K, A), (A, 2, 3), (9, 10, J, Q). Note that set (K, A, 2) would not be a valid sequence, since a given Ace card can only have one of the two ranks, not both.</p>

<p> In addition one of the ranks is chosen to be treated as Jokers, denoted as JK. When constructing sequences, jokers can be used to substitute any rank. For example: (2, JK, 4), (J, Q, JK, A). There can be more than one joker in a single hand. Each of them can be treated as a different rank to be used in a single sequence. Examples: (7, JK, 9, JK, J), (JK, 4, JK, JK, 7). Jokers don't alter the way type (1) sets are build. For example (5, 5, JK) is invalid, but (JK, JK, JK) still can be formed.</p>

<p>Each card has a number of points assigned to it. Ranks 2 to 10 have points equal to their number. A, J, Q, K are 10 points each and Jokers are 0 points. Number of points on a hand is a sum of this hands cards points. The goal of the game is to have minimum number of points after removing some number of sets (possibly none). Help Vishnu find the optimal score for a given hand.</p>

<h3>Input</h3>
<p>Single integer T (1 &lt;= T &lt;= 20) on the first line, the number of test cases. The next T lines contain 14 numbers each, all positive integers not bigger than 13. First 13 describe cards in Vishnu hand and the 14th is the rank chosen to be Jokers. Integers 1, 11, 12, 13 denote A, J, Q, K respectively. There is no upper or lower limit on the number of cards with the same rank, including Jokers. Cards can be freely rearranged to form sets.</p>

<h3>Output</h3>
<p>For each test case output single integer in a separate line: minimum number of points Vishnu can get with a given hand.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
1 2 3 4 5 6 7 8 9 10 11 12 13 3
1 1 3 3 5 5 7 7 9 11 11 13 13 9

<strong>Output:</strong>
0
60</pre>