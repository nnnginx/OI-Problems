<p>
Given an array A having n elements, let X be the maximum sum of any contiguous sequence in the array. How many contiguous sequences in A sum up to X ?
</p>

<h3>Input</h3>
<p>The first line contains T the number of test cases. There follow 2T lines, 2 for each test case. The first line contains the n, the number of elements in the array. The second line contains n space seperated integers Ai.</p>

<h3>Output</h3>
<p>
Output T lines, one for each test case. On each line, output two space seperated integers; the maximum sequence sum, and the number of sequences which obtain this maximum sum.
</p>

<h3>Example</h3>

<p><b>Sample Input</b></p>
<pre>2<br>3<br>-1 -1 -1<br>4<br>2 0 -2 2</pre>

<p><b>Sample Output</b></p>
<pre>-1 3<br>2 4</pre>

<h3>Constraints</h3>
<p><br>1 &lt;= T &lt;= 35<br>1 &lt;= n &lt;= 100000<br>-1000 &lt;= Ai &lt;= 1000</p>