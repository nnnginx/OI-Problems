<p>Here we describe a typical problem. There are <i>n</i> balls and <i>n</i> boxes. Each ball is labeled by a unique
number from 1 to <i>n</i>. Initially each box contains one of these balls. We can swap two balls in adjacent
boxes. We are to sort these balls in increasing order by swaps, i.e. move the ball labeled by 1 to the first
box, labeled by 2 to the second box, and so forth. The question is how many swaps are needed.

</p><p>Now let us consider the situation where the balls are doubled, that is, there are <i>2n</i> balls and <i>n</i> boxes,
exactly two balls are labeled by <i>k</i> for each 1 ¡Ü <i>k</i> ¡Ü <i>n</i>, and the boxes contain two balls each. We can swap
two balls in adjacent boxes, one ball from each box. We are to move the both balls labeled by 1 to the
first box, labeled by 2 to the second box, and so forth. The question is again how many swaps are needed.

</p><p>Here is one interesting fact. We need 10 swaps to sort [5; 4; 3; 2; 1] (the state with 5 in the first box, 4 in
the second box, and so forth): swapping 5 and 4, then 5 and 3, 5 and 2, 5 and 1, 4 and 3, 4 and 2, 4 and
1, 3 and 2, 3 and 1,and finally 2 and 1. Then how many swaps we need to sort [5, 5; 4, 4; 3, 3; 2, 2; 1, 1]
(the state with two 5¡¯s in the first box, two 4¡¯s in the second box, and so forth)? Some of you might think
20 swaps ¡ª this is not true, but the actual number is 15.

</p><p>Write a program that calculates the number of swaps for the two-ball version and verify the above fact.


</p><h3>Input</h3>
<p>The input has the following format:
</p><pre><i>
       n
       ball<sub>1,1</sub> ball<sub>1,2</sub>
       ball<sub>2,1</sub> ball<sub>2,2</sub>
       ...
       ball<sub>n,1</sub> ball<sub>n,2</sub>
</i></pre>
<p><i>n</i> is the number of boxes (1 ¡Ü <i>n</i> ¡Ü 8). ball<sub>i,1</sub> and balli,2 , for 1 ¡Ü <i>i</i> ¡Ü <i>n</i>, are the labels of two balls initially
contained by the <i>i</i>-th box.


</p><h3>Output</h3>
<p>Print the minumum possible number of swaps.

</p><h3>Example</h3>

<pre><b>Input:</b>
5
5 5
4 4
3 3
2 2
1 1

<b>Output:</b>
15
</pre>