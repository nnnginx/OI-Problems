<p>Julia and Robert are playing a game, in which they pick up sticks from heaps. The game starts with <em>n</em> heaps, the <em>i</em>-th heap contains <em>a</em>[<em>i</em>] sticks. In each turn the players choose a heap and take away 2, 3 or 5 sticks from it (removed sticks do not return to the game). Julia starts the game making the first move. The one, who cannot make a move, loses the game, and the other player wins.   Can you decide who will win the game, assuming that both players follow a perfect strategy ? If Julia is the winner, point out her winning move! If there are several possibilities for such a move, then choose the one in which the largest number of sticks is taken away. If there are still several such moves, choose the one, in which sticks are taken from the heap of the smallest number.</p>
<h3>Input</h3>
<p>An integer <em>T</em>, denoting the number of testcases (<em>T</em> &lt;= 1000).  Each testcase contains one integer <em>n</em>, the number of heaps, followed by <em>n</em> non-negative integers: <em>a</em>[1], <em>a</em>[2], ..., <em>a</em>[<em>n</em>], where <em>a</em>[<em>i</em>] is the number of sticks of the <em>i</em>-th heap.</p>
<p>Constraints: <br> 1 &lt;= <em>n</em> &lt;= 1000, <br> 0 &lt;= <em>a</em>[<em>i</em>] &lt;= 1000000000.</p>
<h3>Output</h3>
<p>Please consult the example below for a specification of the required output format. Print a blank line after each testcase.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
1
5
1
7
4
1 2 3 4
10
1 2 3 4 5 6 7 8 9 10
2
1000000 1000001

<strong>Output:</strong>
Julia wins.
Take 5 sticks from heap number 1.

Robert wins.

Julia wins.
Take 3 sticks from heap number 4.

Julia wins.
Take 5 sticks from heap number 6.

Julia wins.
Take 5 sticks from heap number 1.</pre>