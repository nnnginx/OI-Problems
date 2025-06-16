<p>
<a href="http://en.wikipedia.org/wiki/Finite_field">Finite fields</a> only exist when the order (size) is a prime power <em>p<sup>k</sup></em> (where p is a prime number and k is a positive integer). For each prime power, there is a finite field with this size, and all fields of a given order are isomorphic. <br>
Finite fields are fundamental in a number of areas of mathematics and computer science, including number theory, algebraic geometry, Galois theory, finite geometry, cryptography and coding theory.
</p>


<h3>Input</h3>
<p>The first line contains an integer <em>T</em>, the number of test cases.<br>
On the next <em>T</em> lines, you will be given an integer <em>N</em> : a proposed order to be tested.<br>
</p>

<h3>Output</h3>
<p>Output <em>T</em> lines, one for each test case, with <em>p k</em> if <em>N</em> can be the order of a finite field.
<em>p</em> must be a prime number, and <em>k</em> an integer such that <em>N</em>=<em>p<sup>k</sup></em>. Else output "Invalid order".</p>

<h3>Example</h3>
<pre><b>Input:</b>
3
6
7
8

<b>Output:</b>
Invalid order
7 1
2 3
</pre>

<h3>Constraints</h3>
<p>
<em>T</em> about 2<sup>7</sup>, and 1 &lt; <em>N</em> &lt; 2<sup>33333</sup>, <em>N</em> are 2<sup>128</sup>-<a href="http://en.wikipedia.org/wiki/Smooth_number">smooth numbers</a>. (Thanks at <a href="http://www.spoj.com/users/min_25/">Min_25</a> for suggesting this constraint).<br> About 50% of input cases are "Invalid order". <em>N</em> is log-uniform distributed between 2<sup>33333</sup> and its square root.<br>
Prime numbers in <em>N</em> decomposition are almost log-uniform distributed, from 4bit to 128bit. 3 input files.<br>
You may first try <a href="http://www.spoj.com/problems/PRIMEPOW/">PRIMEPOW</a> with easier constraints.<br>
</p>
<p>Edit(2017-02-11) TL updated ; compiler changes.</p>