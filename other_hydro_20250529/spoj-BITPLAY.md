<p>The problem is very <em>simple</em>.</p>
<p><strong>You</strong> are given a even number <strong>N</strong> and an integer <strong>K</strong> and you have to find the greatest odd number <strong>M</strong> less than <strong>N</strong> such that the sum of digits in binary representation of <strong>M</strong> is atmost <strong>K</strong>.</p>

<h3>Input</h3>
<p>For each testcase, you are given an even number <strong>N</strong> and an integer <strong>K</strong>.</p>

<h3>Output</h3>
<p>For each test case, output the integer <strong>M</strong> if it exists, else print <strong>-1</strong>.</p>

<h3>Constraints</h3>
<p>1 &lt;= <strong>T</strong> &lt;= 10^4</p>
<p>2 &lt;= <strong>N</strong> &lt;= 10^9</p>
<p>0 &lt;= <strong>K</strong> &lt;= 30</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
10 2
6 1

<strong>Output:</strong>
9
1</pre>

<h3>Explanation</h3>
<p>First case when <em>N</em> = 10, <em>K</em> = 2</p>
<p>Binary representaion of <strong>10</strong> is <em>1010</em> and binary representation of <strong>9</strong> is <em>1001</em>, hence greatest odd number less than <strong>10</strong> whose sum of digits in its binary representation is atmost <strong>2</strong> is <strong>9</strong>. Hence <em>output</em> is <strong>9</strong></p>