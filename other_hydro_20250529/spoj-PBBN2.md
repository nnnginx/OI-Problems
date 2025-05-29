<p>Some answers for some problems could be huge binary numbers.
In order to check the computation, one could ask you the sum of its digits.
With a little base, the answer is a small number too, but not with a bigger base.</p>

<p>
<a href="http://www.spoj.com/problems/PELLFOUR/">XerK</a> would like to avoid precomputed results and wish check you've computed his huge numbers.
Here's a problem that check computation of a big number N. A <a href="http://www.spoj.com/problems/PBBN1/">tutorial edition</a> exists without language restrictions.</p>

<p>
Let define the function CHK(N, B):<br>
Input  : N a big number in binary representation, B a power of two. Consider N as a base B number.<br>
Output : the sum of its digits in this base.
</p>

<p>
Example :with B=2^8, 12345678 = 78 + 97*B + 188*B*B, so CHK(12345678, B) = 78 + 97 + 188</p>

<p>
This should be easily computed with few bitwise-AND, bitshifts and additions.</p>


<h3>Input</h3>
<p>The input begins with the number T of test cases in a single line.<br>
In each of the next T lines there are four integers A, B, C, D, given in base 10.
</p>

<h3>Output</h3>
<p>For each test case :<br>
* compute N = (A^B) XOR (C^D).<br>
* print CHK(N, 2^16384) as a base 10 number.<br>
(^ denote the power, and XOR the bitwise operator)
</p>


<h3>Example</h3>

<pre><b>Input:</b>
2
7 3 5 4
1234 5678 9012 4444


<b>Output:</b>
806
1194204158794232147799&lt;...snip...&gt;9938532444216215551948305
</pre>

<h3>Explanations</h3>
<p>For test case 1:<br>
7^3 = 343, 5^4 = 625, 343 XOR 625 = 806, CHK(806, 2^16384) = 806.</p>
<p>
For test case 2:<br>
You have to output all 4933 digits of the result.
</p>

<h3>Constraints</h3>
<pre>1 &lt; T &lt;= 321
1 &lt; A, B, C, D &lt;= 10^4
</pre>
<p>Edit 2017-02-11, after compiler update ; new TL. </p>