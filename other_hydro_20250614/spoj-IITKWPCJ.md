<p>Feluda likes strings and mathematics very much. As Feluda is still a child, he was only recently introduced to concept of powers. Being a novice guy, he thinks about powering strings as well as numbers. He defines A^n (A powered to n) to be A + A + ... + A which is a concatenation of n copies of A. For example "bhupkas"^2 = "bhupkasbhupkas".</p>
<p>He wants to check if given two strings A and B, can he find such positive integers n and m so that A ^ n = B ^ m. We are only interested in YES/NO answer, no need to give n and m values.</p>
<p><br></p>

<h3>Input</h3>
<p>First line contains integer T: number of test cases (T &lt;= 100).</p>
<p>Single line per test case containing strings A and B. Both will be non-empty, of lengths of at most 10^5, composed only of lower case letters.</p>
<p><br></p>

<h3>Output</h3>
<p>For each test case, output "YES" if it possible to find integers n and m so that A ^ n = B ^ m or "NO" otherwise (quotes for clarity).</p>
<p><br></p>

<h3>Example</h3>
<pre><strong><u>Input:</u></strong>
3
a a
ab ba
praveen praveen

<strong><u>Output:</u></strong>
YES
NO
YES</pre>