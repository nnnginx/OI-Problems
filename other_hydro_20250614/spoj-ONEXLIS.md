<p>For  a given sequence a[1], a[2], ... a[n], lets call a subsequence a[k<sub>1</sub>],  ...a[k<sub>i</sub>]... a[k<sub>m</sub>] (where 1&lt;=k<sub>i</sub>&lt;=n and k<sub>i</sub>&lt;k<sub>i+1</sub>) as <strong>"one X  increasing subsequence</strong>" if there is exactly one i between 1 and m-1  (inclusive) for which a[k<sub>i</sub>]&gt;a[k<sub>i+1</sub>]. Given a sequence find the  length of the longest "one X increasing subsequence".</p>
<h3>Input</h3>
<p>First line contains t, which denotes the number of test cases. 2*T lines follow. Each test case is described using 2 lines.</p>
<p>First line of a test case contains an integer- n, which denotes the number of elements in the array.</p>
<p>Second lines contains n integers, which represent a[i] 1&lt;=i&lt;=n.</p>
<p>1&lt;=t&lt;=20</p>
<p>1&lt;=n&lt;=100000</p>
<p>1&lt;=a[i]&lt;=10^9</p>
<h3>Output</h3>
<p>For each test case, print one integer which represents the number of integers in the One X LIS. The output for each test case should be printed on a new line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>5<br>4 3 3 4 1<br>5<br>5 4 3 2 1<br><br><strong>Output:</strong>
4<br>2 <br><br><strong>Explanation:</strong></pre>
<p>In the first test case, the Longest Increasing Subsequence is 3.3.4 whereas the longest One X Subsequence is 4.3.3.4 whose length is 4.</p>
<p>In the second example, any two elements can be chosen to form the longest One X Subsequence, which gives us an answer of 2.</p>