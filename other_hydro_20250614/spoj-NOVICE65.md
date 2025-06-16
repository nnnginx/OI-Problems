<p>A derangement of&nbsp;<em>n</em>&nbsp;numbers is a permutation of those numbers in which none of the numbers appears in its original place. For example, the numbers {1,2,3} can be deranged into {2,3,1} and {3,1,2}. We can modify this slightly for&nbsp;<em>n</em>&nbsp;numbers that are not necessarily distinct by saying that no number in the derangement can be in the place that a number of the same value was in in the original ordering. So the numbers {1,1,2,2,3} could be deranged into {2,2,1,3,1}, {2,2,3,1,1}, {2,3,1,1,2}, and {3,2,1,1,2}.</p>
<h3>Input</h3>
<p>First line contains T(1&lt;=T&lt;=100) the number of test cases. Each test case contains two lines. First line contains an integer N(1&lt;=N&lt;=15) denoting total number of elements in the array. Second line contains a space separated list of N integers Ai such that 0&lt;=Ai&lt;N.</p>
<h3>Output</h3>
<p>For each test case output an integer, the total number of derangements of the array.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>2</pre>
<pre>5</pre>
<pre>1 1 2 2 3</pre>
<pre>6</pre>
<pre>0 0 0 1 1 1</pre>
<pre><strong>Output:</strong>
</pre>
<pre>4
</pre>
<pre>1</pre>