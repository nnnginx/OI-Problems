<p>You have an array of size <strong>N </strong>initially filled with 0. You have <strong>Q </strong>queries. In each query, you will be given two integers <strong>a </strong>and <strong>b</strong>. For each query, you need to add <strong>1 </strong>at the following valid indices: ... ... , a - 2*b, a - b, a, a + b, a + 2 * b ... ... The indices that lie in the range <strong>[1,n] </strong>are only considered valid. Print the final array after the last update.&nbsp;</p>
<h3>Input</h3>
<p>The first line contains the number of test cases. Then T test cases follow. Every test case starts with two integers N and Q. After that, Q lines follow. In each line there will be two integers describing that query.&nbsp;</p>
<p>1 &lt;= T &lt;= 10</p>
<p>1 &lt;= N, Q, a, b &lt;= 100000</p>
<h3>Output</h3>
<p>Print the final array after the last query with the case number.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1</pre>
<pre>5 1</pre>
<pre>1 2

<strong>Output:</strong>
Case 1: 1 0 1 0 1</pre>