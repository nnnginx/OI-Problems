<!-- 		@page { margin: 0.79in } 		P { margin-bottom: 0.08in } -->
<p style="margin-bottom: 0in;">You are given K indices, A[1], A[2], ... , A[K].</p>
<p style="margin-bottom: 0in;">A[1] &lt; A[2] &lt; ... &lt; A[K].</p>
<p style="margin-bottom: 0in;">A[1] = 1 and A[K] = N.</p>
<p style="margin-bottom: 0in;">A permutation of the numbers between 1 and N is called valid if :</p>
<p style="margin-bottom: 0in;">The numbers in the permutation between indices A[1] and A[2] (inclusive) form an increasing sequence, the numbers in the permutation between indices A[2] and A[3] (inclusive) form a decreasing sequence, those between A[3] and A[4] (inclusive) form an increasing sequence and so on.</p>
<p style="margin-bottom: 0in;">Count the number of valid permutations.</p>
<p style="text-align: center;"><strong>Input</strong></p>
<!-- 		@page { margin: 0.79in } 		P { margin-bottom: 0.08in } -->
<p style="margin-bottom: 0in;">There will be multiple test cases. The first line contains the number of test cases T.</p>
<p style="margin-bottom: 0in;">There follow 2*T lines, 2 lines for each test case. The first line for each test case contains the numbers N and K. The second line contains K space seperated numbers, ie. A[1] to A[K].</p>
<p>&nbsp;</p>
<p style="text-align: center;"><strong>Output</strong></p>
<!-- 		@page { margin: 0.79in } 		P { margin-bottom: 0.08in } -->
<p style="margin-bottom: 0in;">Output T lines, one for each test case.  All answers should be output MOD 1000000007.</p>
<p style="text-align: center;"><strong>Example</strong></p>
<pre>Sample Input :<br>3
3 3
1 2 3
4 3
1 3 4
10 6
1 2 5 7 8 10<strong><br><br></strong>Sample Output :
2
3
6166<br><br><br><!-- 		@page { margin: 0.79in } 		P { margin-bottom: 0.08in } -->
<p style="margin-bottom: 0in; text-align: center;"><span style="font-family: arial,helvetica,sans-serif;"><strong>Constraints</strong></span></p>
T &lt;= 111
2 &lt;= N &lt;= 20000
2 &lt;= K &lt;= 22<p style="margin-bottom: 0in;">K &lt;= N</p><p style="margin-bottom: 0in;">A[1] &lt; A[2] &lt; ... &lt; A[K].
A[1] = 1 and A[K] = N.</p></pre>