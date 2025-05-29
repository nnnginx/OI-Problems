<p>A particular subgroup of K (1 &lt;= K &lt;= 25,000) of Farmer John's cows likes to make trouble. When placed in a line, these troublemakers stand together in a particular order. In order to locate these troublemakers, FJ has lined up his N (1 &lt;= N &lt;= 100,000) cows. The cows will file past FJ into the barn, staying in order. FJ needs your help to locate suspicious blocks of K cows within this line that might potentially be the troublemaking cows.&nbsp;<br><br>FJ distinguishes his cows by the number of spots 1..S on each cow's coat (1 &lt;= S &lt;= 25). While not a perfect method, it serves his purposes. FJ does not remember the exact number of spots on each cow in the subgroup of troublemakers. He can, however, remember which cows in the group have the same number of spots, and which of any pair of cows has more spots (if the spot counts differ). He describes such a pattern with a sequence of K ranks in the range 1..S. For example, consider this sequence:&nbsp;</p>
<pre>   1 4 4 3 2 1</pre>
<p>In this example, FJ is seeking a consecutive sequence of 6 cows from among his N cows in a line. Cows #1 and #6 in this sequence have the same number of spots (although this number is not necessarily 1) and they have the smallest number of spots of cows #1..#6 (since they are labeled as '1'). Cow #5 has the second-smallest number of spots, different from all the other cows #1..#6. Cows #2 and #3 have the same number of spots, and this number is the largest of all cows #1..#6.&nbsp;<br><br>If the true count of spots for some sequence of cows is:&nbsp;</p>
<pre>   5 6 2 10 10 7 3 2 9</pre>
<p>then only the subsequence 2 10 10 7 3 2 matches FJ's pattern above.&nbsp;<br><br>Please help FJ locate all the length-K subsequences in his line of cows that match his specified pattern.</p>
<h3>Input</h3>
<p>Line 1: Three space-separated integers: N, K, and S&nbsp;<br><br>Lines 2..N+1: Line i+1 describes the number of spots on cow i.&nbsp;<br><br>Lines N+2..N+K+1: Line i+N+1 describes pattern-rank slot i.</p>
<h3>Output</h3>
<p>Line 1: The number of indices, B, at which the pattern matches&nbsp;<br><br>Lines 2..B+1: An index (in the range 1..N) of the starting location where the pattern matches.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
9 6 10
5
6
2
10
10
7
3
2
9
1
4
4
3
2
1

<strong>Output:</strong>
1
3
</pre>