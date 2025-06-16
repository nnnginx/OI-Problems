<p>There are already some SPOJ problems related to <a href="http://en.wikipedia.org/wiki/Pythagorean_triple">Pythagorean triples</a>.  Here is another one: Given an  integer n, calculate the number p(n) of Pythagorean triples with at least one cathetus of length n.</p>
<h3>Input</h3>
<p>Input starts with a positive integer t¡Ü1000, the number of testcases.<br> Each of the following t lines contains a positive integer n¡Ü10<sup>15</sup>.</p>
<h3>Output</h3>
<p>For every n print the value of p(n) in a single line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
4
5
6

<strong>Output:</strong>
1
1
1
</pre>
<p><strong>Explanation</strong>: The only Pythagorean triple that has a cathetus with length 4 is (3,4,5), so p(4)=1.</p>
<p style="font-style:italic"><strong>Note</strong>: If you find the time limit too strict, you may first try the  <a href="../../problems/PTCLONG">tutorial version</a> with identical test data, but increased time limit. I also recommend to solve problems <a href="../../problems/WPC5A">WPC5A</a> and <a href="../../problems/CATHETEN">CATHETEN</a> first.</p>