<p>
The ordinary arithmetical operations of addition, multiplication and exponentiation are naturally extended into a sequence of
<a href="http://en.wikipedia.org/wiki/Knuth's_up-arrow_notation">hyperoperations</a> as follows. </p>
<pre>3¡Á7  = 3 + 3 + 3 + 3 + 3 + 3 + 3 ; there are 7 copies of "3"
3^7  = 3 ¡Á 3 ¡Á 3 ¡Á 3 ¡Á 3 ¡Á 3 ¡Á 3 ; there are 7 copies of "3"
3^^7 = (3^(3^(3^(3^(3^(3^3)))))) ; there are 7 copies of "3"
</pre>
<p>
To extend the sequence of operations beyond exponentiation, Knuth defined a ¡°double arrow¡± operator to denote iterated exponentiation <a href="http://en.wikipedia.org/wiki/Tetration">(tetration)</a> ^^ in ASCII notation.
<br>
This gives us some very big numbers, your task will be to compute modular tetration.
<br>
<strong><em>X</em>^0=1</strong> for all <strong><em>X</em></strong>, as an empty product.
<strong><em>X</em>^^0=1</strong> for all <strong><em>X</em></strong>, for similar reason.
</p>


<h3>Input</h3>
<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.<br>
On each of the next <strong><em>T</em></strong> lines, your are given
three integers <strong><em>X</em></strong>, <strong><em>N</em></strong>, and <strong><em>M</em></strong>.
</p>

<h3>Output</h3>
<p>For each test case, you have to print <strong><em>X^^N modulo M</em></strong>.
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
3 2 20
3 3 345
993306745 75707320 1000000000
</pre>
<pre><strong>Output:</strong>
7
312
884765625
</pre>

<h3>Constraints</h3>
<pre>0 &lt; T &lt;= 10^4
X, N, M unsigned 32bit integers
1 &lt; M
</pre>
<p></p>

<h3>Explanations</h3>
<pre>3^^2 = 3^3 = 27 = 7 [mod 20]
3^^3 = 3^(3^3) = 3^27 = 7625597484987 = 312 [mod 345]
</pre>
<p>Problem designed to be solvable using some 'slow' languages like Python, under half the time limit. (2017-02-11 : TL updated ; compiler changes)<br>
It is recommended to solve first <a href="http://www.spoj.com/problems/POWTOW/">Power Tower City</a>.<br>
;-) Have fun.</p>