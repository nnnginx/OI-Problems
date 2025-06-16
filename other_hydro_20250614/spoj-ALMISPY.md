<p><strong>(3, 4, 5)</strong> is the smallest almost-isosceles Pythagorean triple,
as <strong>4 - 3 = 1</strong>.<br>
Let <strong>S = { (<em>a</em>, <em>a</em>+1, <em>c</em>) | <em>a</em><sup>2</sup> + (<em>a</em>+1)<sup>2</sup> = <em>c</em><sup>2</sup> with <em>a</em> and <em>c</em> positive integers}</strong>.
<br>
One can prove that the set <strong>S</strong> of almost-isosceles Pythagorean triples is infinite.<br>
There is an obvious total order on this set.</p>

<h3>Input</h3>
<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.<br>
On each of the next <strong><em>T</em></strong> lines, your are given
two integers <strong><em>n</em></strong> and <strong><em>m</em></strong>.
</p>

<h3>Output</h3>
<p>For each test case,
you have to find the <strong><em>n</em></strong>th triple
<strong>(<em>a</em>, <em>a</em>+1, <em>c</em>)</strong>
 in the ordered set <strong>S</strong>,
and print <strong><em>a</em></strong> and <strong><em>c</em></strong>.
As the answer could not fit in a 64-bit container, simply output your answer modulo <strong><em>m</em></strong>.
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
1 10
2 123
4 289
</pre>
<pre><strong>Output:</strong>
3 5
20 29
118 118
</pre>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 10^4
0 &lt; n &lt; 10^18
1 &lt; m &lt; 10^9
</pre>
<p><strike>For your information, my 500B-python3 code get AC in 1.61s with 12MB of memory print.<br>
In Python2.7 : (2.49s, 4.0MB), in Python2+psyco (2.04s, 36MB).<br>
My 1kB C code ran in (0.04s, 1.6MB), and time limit is ¡Á125 this one.</strike><br>
<strong>Have fun ;-)</strong><br>
(edit) With wisfaq observation, all my best timings are divided by exactly two!!! <br>
(Edit 2017-02-11, new TL with new compiler. TL 1.11s, in the third (0.37s) my Python3 code ends.)
</p>