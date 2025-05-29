<p align="justify">A function <em>f</em> is defined over natural numbers as:</p>
<p style="font-size:large;">f(N) = ∑ d<sub>i</sub> μ(d<sub>i</sub>)</p>
<p align="justify">Here the summation is over d<sub>i</sub>, all positive integers which are factors of N.</p>
<p align="justify"><em>μ(n)</em> is the <em><a href="http://en.wikipedia.org/wiki/M%C3%B6bius_function">Möbius function</a></em> defined in the following way: If there exists a prime <em>p</em> such that <em>p<sup>2</sup></em> is a factor of <em>n</em>, then <em>μ(n)=0</em>. Otherwise, if <em>n</em> has an odd number of prime factors, <em>μ(n)=-1</em>. If not, <em>μ(n)=1</em>. Thus the first few values for <em>μ(n)</em> (starting from 1) are 1, -1, -1, 0, -1, 1, -1, 0...</p>
<p align="justify">Given an integer X (0 &lt;= X &lt;= 10<sup>12</sup>), find the smallest natural number N such that |f(N)|&gt;X.</p>
<h3>Input</h3>
<p align="justify">The first line of the input contains T, the number of test cases (T &lt;= 1000). Following this are T lines, each containing an integer X (0 &lt;= X &lt;= 10<sup>12</sup>) corresponding to the test case.</p>
<h3>Output</h3>
<p align="justify">For each test case in the input, output the smallest natural number N such that  |f(N)|&gt;X.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
1
2

<strong>Output:</strong>
3
5
</pre>