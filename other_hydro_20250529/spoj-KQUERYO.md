<p>
Given a sequence of n numbers a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>n</sub>&nbsp;and a number of k-queries. 
A k-query is a triple (i, j, k) (1 ¡Ü i ¡Ü j ¡Ü n). For each k-query (i, j, k), you have to return the number of elements <b>greater than</b> k in the subsequence a<sub>i</sub>, a<sub>i+1</sub>, ..., a<sub>j</sub>.
</p>

<h3>Input</h3>
<ul>
  <li>Line 1: n (1 ¡Ü n ¡Ü 30000).</li>
  <li>Line 2: n numbers a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>n</sub>&nbsp;(1 ¡Ü a<sub>i</sub>&nbsp;¡Ü 10<sup>9</sup>).</li>
  <li>Line 3: q (1 ¡Ü q ¡Ü 200000), the number of k- queries.</li>
  <li>In the next q lines, each line contains 3 numbers a, b, c representing a k-query. You should do the following:
  <ul>
    <li>i = a xor last_ans</li>
    <li>j = b xor last_ans</li>
    <li>k = c xor last_ans</li>
  </ul>
  After that 1 ¡Ü i ¡Ü j ¡Ü n, 1 ¡Ü k ¡Ü 10<sup>9</sup> holds.<br>
  Where last_ans = the answer to the last query (for the first query it's 0).</li>
</ul>

<h3>Output</h3>
<p>For each k-query (i, j, k), print the number of elements greater than k in the subsequence a<sub>i</sub>, a<sub>i+1</sub>, ..., a<sub>j</sub>&nbsp;in a single line. </p>

<h3>Example</h3>
<pre><strong>Input:</strong>
6
8 9 3 5 1 9
5
2 3 5
3 3 7
0 0 11
0 0 2
3 7 4

<strong>Output:</strong>
1
1
0
0
2</pre>

<p>[<b>Edited by EB</b>]</p>
There are invalid queries. Assume the following:
<ul>
  <li>if i &lt; 1: i = 1</li> 
  <li>if j &gt; n: j = n</li>
  <li>if i &gt; j: ans = 0</li>
</ul>