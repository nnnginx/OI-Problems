<p>Given 3 positive integers <i>x</i>, <i>y</i> and <i>z</i>, you can find <i>k = x<sup>y</sup>%z</i> easily, by fast power-modulo algorithm. Now your task is the inverse of this algorithm. Given 3 positive integers <i>x</i>, <i>z</i> and <i>k</i>, find the smallest non-negative integer <i>y</i>, such that <i>k%z = x<sup>y</sup>%z</i>.</p>

<h3>Input</h3>
<p>About 600 test cases.
</p><p>Each test case contains one line with 3 integers <i>x</i>, <i>z</i> and <i>k</i>.(1&lt;= <i>x</i>, <i>z</i>, <i>k</i> &lt;=10<sup>9</sup>)
</p><p>Input terminates by three zeroes.</p>

<h3>Output</h3>
<p>For each test case, output one line with the answer, or "No Solution"(without quotes) if such an integer doesn't exist.</p>

<h3>Example</h3>
<pre><b>Input:</b>
5 58 33
2 4 3
0 0 0

<b>Output:</b>
9
No Solution
</pre>