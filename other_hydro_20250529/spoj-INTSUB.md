<p>You are given a set X = {1, 2, 3, 4, бн , 2n-1, 2n} where n is an integer. You have to find the number of interesting subsets of this set X.</p>
<p>A subset of set X is interesting if there are at least two integers a &amp; b&nbsp; such that b is a multiple of a, i.e. remainder of b divides by a is zero and a is the smallest number in the set.</p>
<h3>Input</h3>
<p>The input file contains multiple test cases. The first line of the input is an integer T(&lt;=30) denoting the number of test cases. Each of the next T lines contains an integer 'n' where 1&lt;=n&lt;=1000.</p>
<h3>Output</h3>
<p>For each test case, you have to output as the format below:</p>
<p>Case X: Y&nbsp;</p>
<p>Here X is the test case number and Y is the number of subsets. As the number Y can be very large, you need to output the number modulo 1000000007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3</pre>
<pre>1</pre>
<pre>2</pre>
<pre>3

<strong>Output:</strong>
Case 1: 1</pre>
<pre>Case 2: 9</pre>
<pre>Case 3: 47</pre>