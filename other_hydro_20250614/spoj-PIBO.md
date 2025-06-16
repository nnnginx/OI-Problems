<p>Define a sequence <i>Pib</i>(n) as following </p>
<ul>
<li><i>Pib</i>(0) = 1</li>
<li><i>Pib</i>(1) = 1</li>
<li>otherwise, <i>Pib</i>(n) = <i>Pib</i>(n-1) + <i>Pib</i>(n-2) + <b>P</b>(n)</li>
</ul>
<p>Here <b>P</b> is a polynomial.</p>
<p>Given <b>n</b> and <b>P</b>, find <i>Pib</i>(n) modulo 1,111,111,111.</p>

<h3>Input</h3>
<p>First line of input contains two integer <b>n</b> and <b>d</b> (0 ¡Ü <b>n</b> ¡Ü 10<sup>9</sup>, 0 ¡Ü <b>d</b> ¡Ü 100), <b>d</b> is the degree of polynomial. </p>
<p>The second line contains <b>d</b>+1 integers <b>c</b><sub>0</sub>,<b>c</b><sub>1</sub> ¡­ <b>c</b><sub>d</sub>, represent the coefficient of the polynomial(Thus <b>P</b>(x) can be written as ¦²<b>c</b><sub>i</sub>x<sup>i</sup>). 0 ¡Ü <b>c</b><sub>i</sub> ¡Ü 100 and <b>c</b><sub>d</sub> ¡Ù 0 unless d = 0.</p>

<h3>Output</h3>
<p>A single integer represents the answer.

</p><h3>Example</h3>

<pre><b>Input:</b>
10 0
0

<b>Output:</b>
89

<b>Input:</b>
10 0
1

<b>Output:</b>
177

<b>Input:</b>
100 1
1 1

<b>Output:</b>
343742333

</pre>