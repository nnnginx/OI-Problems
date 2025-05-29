<p>You are given a sequence of N random values (s1, s2, s3, s4, . . . . , sN)<br>You have to find a function f(t) = a*t+b such that the Euclidean Distance between <br>the given sequence and the function values where t varies from 1 to N is minimum.</p>
<p>In effect, you have to minimize</p>
<p style="text-align: center;"><img src="/files/gif/f/e/5/fe51c3542db3f26f40202e10e8ef5b31/"></p>
<p>Output the values a and b for each test case, rounded up to 4 decimal places.</p>
<p><strong>Input</strong></p>
<p>Line 1: T /* Number of test cases T &lt;= 1000 */<br>Line 2: N /* Number of values in first test case N &lt;= 10000 */<br>Line 3: s1 s2 s3 s4 бн sN /* all values are less than 10000 and integers */<br>.<br>.<br>.</p>
<h3>Output</h3>
<p>a b&nbsp; /* Output the values a and b rounded up to 4 decimal places for each test case */</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>3<br>1 1 1<br>3<br>1 2 3<br>3<br>1 3 1

<strong>Output:</strong>
0.0000 1.0000<br>1.0000 0.0000<br>0.0000 1.6667
</pre>