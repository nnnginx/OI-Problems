<p>You are given n numbers a1, a2, , , an. You have to permute the numbers in such a way that resulting permutation should be lexicographically smallest . But there is a problem, you can not swap every pair of numbers. You can only swap the position i and j if they are good position. You will be given m pairs of i and j's which will denote good positions.</p>
<p>So complying to restrictions posed here, find the lexicographically smallest permutation of a1, a2, , , an.</p>
<p>Definition:&nbsp; (a1, a2. ... an) is lexicographically smaller than (b1, b2. .. bn) if first index i where ai and bi differs, ai &lt; bi satisfies.</p>
<p>eg. (1, 2, 3, 4) is smaller than (2, 1, 3, 4)</p>
<h3>Input</h3>
<p>T : number of test cases (T &lt;= 10)</p>
<p>Next Line will contain n and m. (1 &lt;= n &lt;= 10^3 and 0 &lt;= m &lt;= min (n * (n - 1) / 2, 10^5).</p>
<p>Next Line will contains a1, a2, , , an. (a[i] &gt;= 1 &amp;&amp; a[i] &lt;=10^6)</p>
<p>For next m lines, each line will contain i, j seperated by space which will denote that you can swap ai and aj.</p>
<h3>Output</h3>
<p>For each test case, output n numbers representing the permutation of a1, a2, , , an according to problem statement.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>3 1<br>3 2 1<br>2 3<br>4 2<br>2 4 3 1<br>1 3<br>3 4<br><strong>Output:</strong>
3 1 2<br>1 4 2 3</pre>