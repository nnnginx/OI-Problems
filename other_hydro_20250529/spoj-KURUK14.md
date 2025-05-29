<p>A Genie Sequence is a sequence in which every element indicates the number of elements present before or after it. Given an array of numbers, find whether you can form a Genie sequence or not.</p>

<h3>Input</h3>
<p>First line contains a single integer T, the number of test cases. It is followed by T cases each of which contains two lines. First line of each test case contains a single integer N. The next line contains N integers separated by a single space.</p>

<h3>Output</h3>
<p>For each test case output a single line containing "<code>YES</code>" (without quotes) if it is possible to form a genie sequence or "<code>NO</code>" (without quotes)&nbsp;if it is not possible.</p>

<h3>Constraints</h3>
<p>1 &lt;= T &lt;= 20</p>
<p>2 &lt;= N &lt;= 1000</p>
<p>1 &lt;= ai &lt;= 1000</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1
4
1 3 3 2

<b>Output:</b>
YES</pre>

<h4>Explanation for the test case:</h4>
<p>The Genie sequence is {3, 1, 2, 3}. The first element '3' in the sequence indicates that three numbers are after it, the 2nd element '1' indicates that one number if before it, the 3rd element '2' indicates that two elements are before it and the last element indicates that three elements are before it. So the answer is YES.</p>