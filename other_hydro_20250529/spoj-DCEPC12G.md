<p>Prime(<strong>n</strong>) is defined as&nbsp; number of primes less than equal to <strong>n</strong>.</p>
<p>Totient(<strong>n</strong>) is defined as the number of positive integers less than or equal to&nbsp;<strong>n</strong>&nbsp;that are&nbsp;relatively prime&nbsp;to&nbsp;<strong>n</strong>.</p>
<p>F(<strong>n</strong>) = Prime(<strong>n</strong>) ¨C Totient(<strong>n</strong>)&nbsp;</p>
<p>and we don¡¯t like negative values, so if F(<strong>n</strong>) &lt; 0, consider it as 0.</p>
<p>G(n) = Totient(<strong>n</strong>) ^ (Factorial (F(<strong>n</strong>)))</p>
<p>&nbsp;</p>
<p>You are given a number <strong>n</strong>. You have to output G(<strong>n</strong>) % 10^9+7.</p>
<h3>Input</h3>
<p>First line consists of <strong>T</strong>, the number of test cases.</p>
<p>Each of the next <strong>T</strong> lines contains one integer <strong>n</strong>.</p>
<h3>Output</h3>
<p>Output <strong>T</strong> lines each line containing the value of function G(<strong>n</strong>) % 10^9+7</p>
<h3>Constraints</h3>
<p>1&lt;=<strong>T</strong>&lt;=100</p>
<p>1&lt;=<strong>n</strong>&lt;=10000000</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1</pre>
<pre>2

<strong>Output:</strong>
1</pre>