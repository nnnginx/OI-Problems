<p>Given <strong><em>P</em></strong> a prime number, and <strong><em>N</em></strong> an integer, <a href="http://www.spoj.com/problems/DUKKAR/">Dukkar</a> found a really fast way to compute how many numbers are divisible by <strong><em>P</em></strong> on the <strong><em>N</em></strong><sup>th</sup> row of the Pascal triangle.
Now the task will be much harder : it's for all the <strong><em>N</em></strong> first rows.<br>
Moreover <strong><em>N</em></strong> will be a giant number, given in base <strong><em>P</em></strong> for convenience.</p>

<h3>Input</h3>
<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases. Follow 2¡Á<strong><em>T</em></strong> lines.<br>
For each test case, on the first line your are given two integers <strong><em>P</em></strong> and <strong><em>k</em></strong>.<br>
On the second line you are given <strong><em>k</em></strong> integers : the digits of <strong><em>N</em></strong> in base <strong><em>P</em></strong>.<br>
<br>
<strong><em>N = a<sub>0</sub>¡ÁP<sup>0</sup> + ... + a<sub>i</sub>¡ÁP<sup>i</sup> + ... + a<sub>k-1</sub>¡ÁP<sup>k-1</sup> </em></strong>
</p>

<h3>Output</h3>
<p>For each test case, you have to print the number
 of numbers in all the first <strong><em>N</em></strong> rows of the Pascal triangle that are divisible by <strong><em>P</em></strong>.
As the answer could not fit in a 64bit container, give your answer modulo 1000000007.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
5 2
0 1 
5 2
1 1
7 3
2 0 2
</pre>
<pre><strong>Output:</strong>
0
4
2689
</pre>
<h3>Explanations</h3>
<p>For the first case, N = 0¡Á5<sup>0</sup> + 1¡Á5<sup>1</sup> = 5. No numbers are divisible by 5 in the first 5 rows.<br>
For the second case, N = 1¡Á5<sup>0</sup> + 1¡Á5<sup>1</sup> = 6. Only 4 numbers are divisible by 5 in the first 6 rows.<br></p>
<pre>1
1 1
1 2 1
1 3 3 1
1 4 6 4 1
1 <b>5 10 10 5</b> 1
</pre>
<p>
For the third case, N = 2¡Á7<sup>0</sup> + 0¡Á7<sup>1</sup> + 2¡Á7<sup>2</sup> = 100.</p>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 300
0 &lt; P &lt; 10^9, a prime number
0 &lt; k &lt; 1000
0 &lt;= a<sub>i</sub> &lt; P,  a<sub>k-1</sub>&gt;0
</pre>
<p>For your information, my 300B-python3 code get AC in 3.03s with 11MB of memory print.<br>
My C-code get AC in 0.08s with 1.6MB of memory print.<br>
<strong>Have fun ;-)</strong>
</p>
<p>Edit(25/I/2015) With Cube cluster my C-time is 0.01s and my PY3.4-time is 0.26s.</p>
<p>Edit(11/II/2017) With compiler changes my C-time is 0.00s and my PY3.4-time is 0.12s.</p>