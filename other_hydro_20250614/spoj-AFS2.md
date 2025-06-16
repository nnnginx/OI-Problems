<h3>Warning</h3>
<p> Here is a harder version of
 <a href="https://www.spoj.com/problems/AFS/" target="next"> Amazing Factor Sequence </a>.</p>
<p>To make things clear, you'll need a O(n^0.5) method to solve this problem.
You'll need to be careful with container of C-like language,
and/or you'll need to find some little optimizations with slower language.
</p>

<h3>The factor sequence</h3>
<p> We define our factor sequence with:</p>

<p> <strong><em>a[0] = a[1] = 0</em></strong>, and</p>
<p>for  <strong><em>n &gt; 1, a[n] = a[n - 1] + sum({x | x &lt; n and n % x = 0})</em></strong>.</p>

<h3>Input</h3>

<p>First line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.</p>

<p> Each of the next <strong><em>T</em></strong> lines contains
 a single integer <strong><em>n</em></strong>.</p>

<h3>Output</h3>
<p>For each test case, print <strong><em>a[n]</em></strong> on a single line.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
3
4
5</pre>
<pre><strong>Output:</strong>
2
5
6</pre>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 101
0 &lt; n &lt; 12148001999
</pre>
<p>Numbers <strong><em>n</em></strong> are uniform-randomly chosen. <strong><em>Nmax</em></strong> was carefully chosen ;-)<br>
Time limit is ¡Á2.5 my python one (2.56s). (Edited 2017-02-11, after compiler changes)</p>