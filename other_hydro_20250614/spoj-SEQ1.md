<p>The input consists of exactly 5 test cases in the following format:</p>
<h3>Input</h3>
<pre>N A0 B0 L0 A1 B1 L1 [3&lt;=N&lt;=1000,1&lt;=A0&lt;=B0&lt;=L0&lt;=N,1&lt;=A1&lt;=B1&lt;=L1&lt;=N]
</pre>
<h3>Output</h3>
<p>Exactly 5 lines,each contains:</p>
<p>a) A N-character sequence (We name it S) consisting of only characters '0' and '1' and no extra whitespaces, which satisfy the following conditions:</p>
<div>
<ul>
<li> The number of '0' in any consecutive subsequence of S whose length is L0 is not more than B0 and not less than A0. </li>
<li> The number of '1' in any consecutive subsequence of S whose length is L1 is not more than B1 and not less than A1.</li>
</ul>
</div>
<p>or</p>
<p>b)A single number -1,if the sequence which satisfies the conditions above doesn't exist.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 1 2 3 1 1 2
[and 4 test cases more]

<strong>Output:</strong>
010101
[and 4 test cases more]
</pre>