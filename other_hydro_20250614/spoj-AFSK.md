<p> Here is a mixed edition of
 <a href="http://www.spoj.com/problems/IITD4/" target="next"> Divisor Summation Powered </a> and <a href="http://www.spoj.com/problems/AFS2/" target="next"> Amazing Factor Sequence (medium)</a>.</p>

<h3>The powered factor sequence</h3>
<p> For <strong><em>k</em></strong> an integer number, we define our powered factor sequence with:</p>

<p> <strong><em>a<sub>k</sub>[0] = 0;  a<sub>k</sub>[1] = 1</em></strong>, and</p>
<p>for  <strong><em>n &gt; 1, a<sub>k</sub>[n] = a<sub>k</sub>[n - 1] + sum({x^k | 0 &lt; x ¡Ü n and n % x = 0})</em></strong>.</p>

<h3>Input</h3>

<p>First line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.</p>

<p> Each of the next <strong><em>T</em></strong> lines contains
 three integers <strong><em>n, k, m</em></strong>.</p>

<h3>Output</h3>
<p>For each test case, print <strong><em>a<sub>k</sub>[n]</em></strong> on a single line.<br>
As the answer could be a big number, you just have to output it modulo <strong><em>m</em></strong>. </p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
3 1 10
4 2 55
5 3 97</pre>
<pre><strong>Output:</strong>
8
37
43</pre>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 101
0 &lt; n &lt; 10^9
0 &lt; k &lt; 11
1 &lt; m &lt; 10^17
</pre>
<p>Numbers <strong><em>n, k, m</em></strong> are uniform-randomly chosen.<br>
For your information, there's two input files, the first one is 'easy' with n¡Ü100.<br>
My (1kB)-python code get AC around 0.96s. I have a much slower basic PIKE AC (4.8s).<br>
(Edit 2017-02-11 ; timings and TL updated after compiler changes)
</p>