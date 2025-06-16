<p>You are given a sequence of N integers A<sub>1</sub>, A<sub>2</sub> .. A<sub>N</sub>. (-10000 &lt;= A<sub>i</sub> &lt;= 10000, N &lt;= 50000)
</p>
<p>Let S<sub>i</sub> denote the sum of A<sub>1</sub>..A<sub>i</sub>. You need to apply M (M &lt;= 50000) operations:
</p>

<ul>
<li>0 x y k: increase all integers from A<sub>x</sub> to A<sub>y</sub> by k(1 &lt;= x &lt;= y &lt;= N, -10000 &lt;= k &lt;= 10000).
</li><li>1 x y: ask for max{ S<sub>i</sub> | x &lt;= i &lt;= y }.(1 &lt;= x &lt;= y &lt;= N)
</li></ul>


<h3>Input</h3>
<ul>
<li>In the first line there is an integer N.
</li><li>The following line contains N integers that represent the sequence.
</li><li>The third line contains an integer M denotes the number of operations.
</li><li>In the next M lines, each line contains an operation "0 x y k" or "1 x y".
</li></ul>


<h3>Output</h3>	
<p>For each "1 x y" operation, print one integer representing its result.
</p>



<h3>Example</h3>

<pre><b>Input:</b>
5
238 -9622 5181 202 -6943
5
1 3 4
0 5 5 4846
1 3 5
0 3 5 -7471
1 3 3

<b>Output:</b>
-4001
-4001
-11674</pre>

<p><b>Use signed 64-bit integer :)</b></p>