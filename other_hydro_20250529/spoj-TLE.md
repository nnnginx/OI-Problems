<p>Given integers N (1 ¡Ü N ¡Ü 50) and M (1 ¡Ü M ¡Ü 15), compute the number of sequences a<sub>1</sub>, ..., a<sub>N</sub> such that:</p>

<ul>
<li>0 ¡Ü a<sub>i</sub> &lt; 2<sup>M</sup></li>
<li>a<sub>i</sub> is not divisible by c<sub>i</sub> (0 &lt; c<sub>i</sub> ¡Ü 2<sup>M</sup>)</li>
<li>a<sub>i</sub> &amp; a<sub>i+1</sub> = 0 (that is, a<sub>i</sub> and a<sub>i+1</sub> have no common bits in their binary representation)</li>
</ul>

<h3>Input</h3>
<p>The first line contains the number of test cases, T (1 ¡Ü T ¡Ü 10). For each test case, the first line contains the integers N and M, and the second line contains the integers c<sub>1</sub>, ..., c<sub>N</sub>.</p>

<h3>Output</h3>
<p>For each test case, output a single integer: the number of sequences described above, modulo 1,000,000,000.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
2 2
3 2

<b>Output:</b>
1
</pre>

<p>The only possible sequence is 2, 1.</p>
<h3><b>time limit has been doubled, enjoy :D</b></h3>