<p style="text-align: justify;">Vaibhav loves playing with numbers. To enjoy his summer holidays he decides to join the group "number players" of his school. He decides to visit the group hall. At the gate he finds a lock and a paper. The gate can only be unlocked by solving the puzzle written on the paper. Vaibhav is stuck with his puzzle, help him in solving it.<br><br>Here is the puzzle description:<br><br>Given a sequence F(N)<br><br>F(0)=1<br><br>F(1)=1<br><br>F(2)=1<br><br>F(n) = product of all odd primes less than or equal to n (for n&lt;=10)<br><br>F(n) = (2^(n/4)) * F(n/5)* F(n/10) &nbsp; &nbsp; &nbsp;(for n&gt;10)</p>
<p style="text-align: justify;"><strong>For every fraction , a ceil value is taken for evaluation.</strong></p>
<p style="text-align: justify;"><strong> For eg. F(11)=2^ceil(11/4) * F(ceil(11/5)) * F(ceil(11/10))&nbsp; = 2^3 * F(3) * F(2) = 24</strong><br><br>Given N. Find the max value of <strong>(a^b)%mod</strong> such that a and b satisfies the relation gcd(a,b) = F(N).<br><br>Gcd : Greatest common divisor</p>
<h3>Input</h3>
<p>First line gives T, total number of testcases.<br><br>Next T line gives number N</p>
<h3>Output</h3>
<p>For each test case, print the desired value on a new line</p>
<h3>Constraints</h3>
<p>T&lt;=10<br><br>N&lt;=10^6</p>
<p>mod = 10^9.</p>
<p>NOTE: a must be &lt;= 5*F(n) and b must be &lt;=5*F(n) , a can be equal to b and mod=10^9</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1<br>2<br><br><strong>Output:</strong>
1024</pre>