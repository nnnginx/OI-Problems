<p>Define a sequence&nbsp;<em>Pib</em>(n) as following</p>
<ul>
<li><em>Pib</em>(0) = 1</li>
<li><em>Pib</em>(1) = 1</li>
<li>otherwise,&nbsp;<em>Pib</em>(n) =&nbsp;<em>Pib</em>(n-1) +&nbsp;<em>Pib</em>(n-2) +&nbsp;<strong>P</strong>(n)</li>
</ul>

<p>Here&nbsp;<strong>P</strong>&nbsp;is a polynomial.</p>
<p>Given&nbsp;<strong>n</strong>&nbsp;and&nbsp;<strong>P</strong>, find&nbsp;<em>Pib</em>(n) modulo 1,111,111,111.</p>
<p>Maybe you should solve <a href="../PIBO/">PIBO</a>&nbsp;before this task, it has lower constraints.</p>

<h3>Input</h3>
<p>First line of input contains two integer&nbsp;<strong>n</strong>&nbsp;and&nbsp;<strong>d</strong>&nbsp;(0 ¡Ü&nbsp;<strong>n</strong>&nbsp;¡Ü 10<sup>9</sup>, 0 ¡Ü&nbsp;<strong>d</strong>&nbsp;¡Ü 10000),&nbsp;<strong>d</strong>&nbsp;is the degree of polynomial.</p>
<p>The second line contains&nbsp;<strong>d</strong>+1 integers&nbsp;<strong>c</strong><sub>0</sub>,<strong>c</strong><sub>1</sub>&nbsp;¡­&nbsp;<strong>c</strong><sub>d</sub>, represent the coefficient of the polynomial (Thus&nbsp;<strong>P</strong>(x) can be written as ¦²<strong>c</strong><sub>i</sub>x<sup>i</sup>). 0 ¡Ü&nbsp;<strong>c</strong><sub>i</sub>&nbsp;&lt; 1,111,111,111 and&nbsp;<strong>c</strong><sub>d</sub>&nbsp;¡Ù 0 unless d = 0.</p>

<h3>Output</h3>
<p>A single integer represents the answer.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
10 0
0

<strong>Output:</strong>
89

<strong>Input:</strong>
10 0
1

<strong>Output:</strong>
177

<strong>Input:</strong>
100 1
1 1

<strong>Output:</strong>
343742333
</pre>