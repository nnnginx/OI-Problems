<p>Consider the following pseudo-code</p>
<p>int a[1..N];&nbsp;</p>
<p>int max = -1;</p>
<p>for i = 1..N:</p>
<p><span style="white-space: pre;"> </span>if(a[i] &gt; max)&nbsp;</p>
<p><span style="white-space: pre;"> </span>max = a[i];</p>
<p>&nbsp;</p>
<p>Your task is to calculate the expected number of times the 'if' block of the above pseudo-code executes. The array 'a' is a random permutation of numbers from 1..N chosen uniformly at random.&nbsp;</p>
<h3>Input</h3>
<p>First line contains t, the number of test cases. t lines follow, each containing N, the number of elements in the array.</p>
<p>1&lt;= t &lt;= 100</p>
<p>1&lt;= n &lt;=100,000</p>
<h3>Output</h3>
<p>For each test case, output a single decimal. Your answer should be within 10^-6 of the correct answer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1</pre>
<pre>2

<strong>Output:</strong>

</pre>
<pre>1.5</pre>
<pre>Explaination :</pre>
<pre>for N=2, you can have the following two permutations: [1,2]  and [2,1] . </pre>
<pre>for the first case the if block gets executed 2 times and for the second one the if block gets executed 1 time. So the expected </pre>
<pre>value is (3)/2 = 1.5</pre>