<p>You are given N number a<sub>1</sub>, a<sub>2</sub>, ... , a<sub>N</sub>. In a <em>segment flip</em>, you can pick a contiguous segment a<sub>i</sub>, a<sub>i+1</sub>, ... , a<sub>j</sub>&nbsp;of these numbers, where i&lt;=j and negate all the numbers in this segment.&nbsp;</p>

<p>You are permitted atmost K segment flip&nbsp;operations overall. Also, no 2 segments that you pick can overlap. That is, if you flip a<sub>i</sub>, ... , a<sub>j</sub>&nbsp;and a<sub>k</sub>, ... , a<sub>l</sub>&nbsp;then either j &lt; k or l &lt; i.</p>

<p>Your aim is to maximize the sum of all the numbers in the resulting sequence by applying appropriate segment flip operations meeting these constraints.</p>

<p>For instance, suppose the sequence is -5, 2, -3 and you are allowed a single segment flip. The best sum you can achieve is 6, by flipping all 3 numbers as a single segment to 5, -2, 3.</p>

<h3>Input</h3>
<p>The first line contains 2 integers N and K. The next line contains N integers, the initial values of a<sub>1</sub>, a<sub>2</sub>, ... , a<sub>N</sub>.</p>

<h3>Output</h3>
<p>A single integer denoting the maximum possible sum of the final array.</p>

<h3>Constraints</h3>
<p>
0 &lt;= K &lt;= N<br>
-10000 &lt;= a<sub>i</sub>&nbsp;&lt;= 10000<br>
1 &lt;= N &lt;= 100000
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3 1
-5 2 -3

<strong>Output:</strong>
6</pre>