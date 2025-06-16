<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/ROADS/en/">English</a></td>
<td width="50%"><a href="/problems/ROADS/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>N cities named with numbers 1 ... N are connected with one-way roads. Each road has two parameters associated with it: the road length and the toll that needs to be paid for the road (expressed in the number of coins). Bob and Alice used to live in the city 1. After noticing that Alice was cheating in the card game they liked to play, Bob broke up with her and decided to move away - to the city N. He wants to get there as quickly as possible, but he is short on cash. We want to help Bob to find the shortest path from the city 1 to the city N that he can afford with the amount of money he has.</p>
<h3>Input</h3>
<p>The input begins with the number t of test cases. Then t test cases follow. The first line of the each test case contains the integer K, 0 &lt;= K &lt;= 10000, maximum number of coins that Bob can spend on his way. The second line contains the integer N, 2 &lt;= N &lt;= 100, the total number of cities. The third line contains the integer R, 1 &lt;= R &lt;= 10000, the total number of roads. Each of the following R lines describes one road by specifying integers S, D, L and T separated by single blank characters : S is the source city, 1 &lt;= S &lt;= N D is the destination city, 1 &lt;= D &lt;= N L is the road length, 1 &lt;= L &lt;= 100. T is the toll (expressed in the number of coins), 0 &lt;= T &lt;= 100 Notice that different roads may have the same source and destination cities.</p>
<h3>Output</h3>
<p>For each test case, output a single line contain the total length of the shortest path from the city 1 to the city N whose total toll is less than or equal K coins. If such path does not exist, output -1.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
5
6
7
1 2 2 3
2 4 3 3
3 4 2 4
1 3 4 1
4 6 2 1
3 5 2 0
5 4 3 2
0
4
4
1 4 5 2
1 2 1 0
2 3 1 1
3 4 1 0

<strong>Output:</strong>
11
-1
</pre>
<p> </p>