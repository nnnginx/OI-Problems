<p>You are given a sequence A of N (N &lt;= 50000) integers between -10000 and 10000. On this sequence you have to apply M (M &lt;= 50000) operations: <br>
modify the i-th element in the sequence or for given x y print max{Ai + Ai+1 + .. + Aj | x&lt;=i&lt;=j&lt;=y }.
</p><h3>Input</h3>
<p>The first line of input contains an integer N. The following line contains N integers, representing the sequence A1..AN. <br>
The third line contains an integer M. The next M lines contain the operations in following form:<br>
0 x y: modify Ax into y (|y|&lt;=10000).<br>
1 x y: print max{Ai + Ai+1 + .. + Aj | x&lt;=i&lt;=j&lt;=y }.<br>
</p><h3>Output</h3>
<p>For each query, print an integer as the problem required.
</p><h3>Example</h3>

<pre><b>Input:</b>
4
1 2 3 4
4
1 1 3
0 3 -3
1 2 4
1 3 3

<b>Output:</b>
6
4
-3
</pre>