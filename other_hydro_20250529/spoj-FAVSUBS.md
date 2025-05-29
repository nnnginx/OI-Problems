<table border="0">
<tbody>
<tr>
<td>
<p><img src="./22391/file/MAEJZFmU.png" border="0" alt="" width="221" height="185"></p>
</td>
<td>
<p align="justify">Little Princess Rapunzel is blessed with long (really looong!) hair, which is golden colored and has healing power. After the end of a long happy story, she marries her lover Flynn. They decide to lead a normal life by getting rid of the mysterious hair, which when cut loses its power and turns brown. There are many colorful beads on her hair in order. Rapunzel has some <strong>K</strong> favorite colors <strong>B</strong>[1...K] <br><br> To remember good old stories, she wants to keep a part of her hair after its cut. A favorite sub hair is that continuous part of the hair, which has each of her favorite color beads at least once.</p>
</td>
</tr>
</tbody>
</table>
<p align="justify">For the purpose of this problem, we represent a color as an integer and Hair as an array <strong>A</strong>[1...N], which has exactly <strong>N</strong> colored beads in the given order. Could you please tell her the total number of ways she can cut her favorite sub hair (sub-array). Two sub-arrays are different, if their starting or ending index in A differ.</p>
<h3>Input</h3>
<p>First line contains T [ number of test cases, around 10 ]. Each test case is preceded by a blank line, including the 1st case. [ -2,000,000 &lt;= A[i], B[j] ( colors ) &lt;= 2,000,000 ]<br> Each test case has 4 lines, as described below.<br> N [ 1 &lt;= N &lt;= 100,000 ]<br> &lt; Array A : N integers, separated by spaces &gt;<br> K [ 1 &lt;= K &lt;= 1,000 ]<br> &lt; Array B : K integers, separated by spaces, her favorite colors, without repetition &gt;</p>
<h3>Output</h3>
<p>For each test case, output the number of different sub-arrays, which has her favorite color appearing at least once, in a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3

4
1 2 3 1
2
1 2

6
10 20 30 40 50 60
1
20

5
1 2 3 4 5
2
2 6

<strong>Output:</strong>
4
10
0

<strong>Explanation:</strong>
Case 1 : Favorite sub-arrays in bold [ <strong>1 2</strong> 3 1 ], [ <strong>1 2 3</strong> 1 ] , [ 1 <strong>2 3 1</strong> ], [ <strong>1 2 3 1</strong> ]
</pre>
<p><br> Note: Large input, prefer using scanf / printf to cin / cout<br><br> <em>There are multiple test sets, and the judge shows the <strong>sum</strong> of the time taken over all test sets of your submission, if Accepted.</em></p>