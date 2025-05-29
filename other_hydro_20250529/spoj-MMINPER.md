<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MMINPER/en/">English</a></td> 
<td width="50%"><a href="/problems/MMINPER/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<pre>The inversion number of an integer sequence a1, a2, . . . , an is the number
of pairs (ai, aj) that satisfy i &lt; j and ai &gt; aj . Given n and the inversion
number m, your task is to ﬁnd the smallest permutation of the set { 1, 2, . . . , n } , 
whose inversion number is exactly m. A permutation a1, a2, . . . , an is smaller 
than b1, b2, . . . , bn if and only if there exists an integer k such that aj = bj 
for 1 ≤ j &lt; k but ak &lt; bk.
</pre>
 
<h3>Input</h3>
<pre>The input consists of several test cases. Each line of the input contains two
integers n and m. Both of the integers at the last line of the input is −1,
which should not be processed. You may assume that
1 ≤ n ≤ 50000 and 0 ≤ m ≤ 1/2n(n − 1).

Sample Input
5 9
7 3
-1 -1
</pre>

<h3>Output</h3>
<pre> 
For each test case, print a line containing the smallest permutation as 
described above, separates the numbers by single spaces.

Sample output
4 5 3 2 1
1 2 3 4 7 6 5
</pre>