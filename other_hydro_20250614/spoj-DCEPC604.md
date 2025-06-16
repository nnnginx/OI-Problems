<p>Now you all helped Vaibhav solve the puzzle and open the gate last time (although not<br>too much help). But as soon as he opens the gate, there is another puzzle to open the front door. Let¡¯s see whether this time you all are able to help him or not.</p>
<p>Fac(n) = no of zeroes in n!<br>Fact(n)= Fac(n)%25+1<br><br> F(0)=1<br><br> F(1)=1<br><br> F(2)=1<br><br> F(n) = product of all odd primes less than or equal to n (for n&lt;=10)<br><br> F(n) = 4^fact(n) * f(n/5) * f(n/10) &nbsp; (for n&gt;10)</p>
<p>&nbsp;</p>
<p style="text-align: justify;"><strong>For every fraction , a floor value is taken for evaluation.</strong></p>
<p style="text-align: justify;"><strong>For eg. F(11)=4^fact(11) * F(floor(11/5)) * F(floor(11/10))&nbsp; = 4^3 * F(2) * F(1) = 64</strong><br><br>Given N. Find the max value of&nbsp;<strong>(a^b)%mod</strong>&nbsp;such that a and b satisfies the relation gcd(a,b) = F(N).<br><br>Gcd : Greatest common divisor</p>
<h3>Input</h3>
<p>First line gives T, total number of testcases.<br>Next T line gives number N</p>
<h3>Output</h3>
<p>For each test case, print the desired value on a new line.</p>
<h3>Constraints</h3>
<p>T&lt;=10<br><br>N&lt;=10^6</p>
<p>mod = 10^9.</p>
<p>NOTE: a must be &lt;= 5*F(n) and b must be &lt;=5*F(n) , a can be equal to b and mod=10^9</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<br>1</pre>
<pre><span class="AM">2</span>&nbsp;

<strong>Output:</strong>
<br>1024
</pre>