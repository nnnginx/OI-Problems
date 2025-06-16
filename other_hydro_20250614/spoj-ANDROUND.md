<p>You are given a cyclic array A having N numbers. In an AND round, each element of the array A is replaced by the bitwise AND of itself, the previous element, and the next element in the array. All operations take place simultaneously. Can you calculate A after K such AND rounds ?</p>

<h3>Input</h3>
<p>
The first line contains the number of test cases T (T &lt;= 50). <br>There follow 2T lines, 2 per test case. The first line contains two space seperated integers N (3 &lt;= N &lt;= 20000) and K (1 &lt;= K &lt;= 1000000000). The next line contains N space seperated integers Ai (0 &lt;= Ai &lt;= 1000000000), which are the initial values of the elements in array A.
</p>
<h3>Output</h3>
<p>
Output T lines, one per test case. For each test case, output a space seperated list of N integers, specifying the contents of array A after K AND rounds.
</p>
<h3>Example</h3>
<pre><b>Sample Input:</b>
2 
3 1 
1 2 3 
5 100 
1 11 111 1111 11111 
 
<b>Sample Output:</b>
0 0 0 
1 1 1 1 1</pre>