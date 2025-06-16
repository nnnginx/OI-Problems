<p>Given <strong>n</strong> integers, your task is to pick <strong>k</strong> out of them so that the picked number are minimum when do bitwise AND among all of them.</p>
<h3>Input</h3>
<p>There are multiple test cases for this problem. The first line of the input contains an integer denoting the number of test cases.</p>
<p>For each test case, there are two integers in the first line: <strong>n</strong> and <strong>k</strong>, denoting the number of given integers and the number of integers you are asked to pick out. (1&lt;= <strong>n</strong> &lt;=40, 1&lt;= <strong>k</strong> &lt;= <strong>n</strong>)</p>
<p>The second line contains the n integers. You may assume that all integers are smaller than 2<sup>60</sup>.</p>
<p><em>Note: There are about one thousand randomly generated test cases. Fortunately 90% of them are relatively small.</em></p>
<h3>Output</h3>
<p>For each test case, output only one integer - the smallest possible value.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 2
5 6 7
8 2
238 153 223 247 111 252 253 247

<strong>Output:</strong>
Case #1: 4
Case #2: 9
</pre>