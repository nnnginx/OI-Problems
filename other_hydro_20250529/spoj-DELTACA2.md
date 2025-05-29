<p><strong>(3, 4, 5)</strong> is a famous Pythagorean triple,
it gives a quick answer to the question:<br>

For a given integer <strong><em>d</em></strong>, is there a Pythagorean triple
 <strong>(<em>a, b, c</em>)</strong> such that <strong><em>b - a = d</em></strong>?</p>


<p>
A solution is <strong>(3<em>d</em>, 4<em>d</em>, 5<em>d</em>)</strong>,
 and in fact one can easily prove that the set of solutions is infinite, and
that there is an obvious total order on those solutions.<br>
Given <strong><em>n</em></strong>, you'll have to find the
 <strong><em>n</em></strong>th term of the sequence of solutions.
</p>

<p>Geometrically, it is the study of right angle triangles for which the difference of the
catheti is equal to <strong><em>d</em></strong>.</p>

<h3>Input</h3>

<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.</p>
<p><strong>2<em>T</em></strong> lines follow. Each case is on two lines.<br>
The first line of the case contains
 three integers <strong><em>n, d, m</em></strong>.<br>
The second line contains an integer <strong><em>L</em></strong> and
 <strong>2<em>L</em></strong> other integers (p, e) ; this gives the prime factorization of <strong><em>d</em></strong> in standard format (d = product p^e).</p>

<h3>Output</h3>
<p>For each test case, compute the <strong><em>n</em></strong>th term amongst
the solutions <strong>(<em>a, b, c</em>)</strong> for the problem :<br>
<strong><em>a<sup>2</sup> + b<sup>2</sup> = c<sup>2</sup></em></strong> with <strong><em>b - a = d</em></strong>
and <strong><em>0 &lt; a &lt; b &lt; c </em></strong>.</p>
<p>As the answer could not fit in a 64-bit container, simply output your answer modulo <strong><em>m</em></strong>.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
1 1 235813
0
3 21 1000
2 3 1 7 1
9 119 11
2 7 1 17 1
</pre>
<pre><strong>Output:</strong>
3 4 5
63 84 105
5 3 1
</pre>

<h3>Explanations</h3>
<p>For the first case, the first solution is <strong>(3, 4, 5)</strong>, as 4 - 3 = 1.</p>
<p>For the second case, the first solutions are:<br>
<strong>(15, 36, 39), (24, 45, 51), (63, 84, 105), (144, 165, 219), (195, 216, 291), (420, 441, 609), ...</strong><br>
The third one is <strong>(63, 84, 105)</strong>.</p>
<p>For the third case, the first solutions are:<br>
<strong>(24, 143, 145), (49, 168, 175), (57, 176, 185), (85, 204, 221), (136, 255, 289),
 (180, 299, 349), (196, 315, 371), (261, 380, 461), (357, 476, 595), (481, 600, 769),
 (616, 735, 959), ... </strong><br>
The 9th solution is <strong>(357, 476, 595)</strong>, reduced modulo 11, we get
<strong>(5, 3, 1)</strong>.

</p>
<h3>Constraints</h3>
<pre>0 &lt; T &lt; 10^4
0 &lt; n &lt; 10^18
0 &lt; d &lt; 10^14
1 &lt; m &lt; 10^9
</pre>
<p><strong><em>d</em></strong> is the product of two integers lower than 10^7.<br>
<strong><em>n, d<sub>1</sub>, d<sub>2</sub>, m</em></strong> : Uniform randomly chosen in their range.<br>
Those constraints are set to allow C-like users to work only with 64bit containers.</p>
<p>For your information, my 3kB-python3 code get AC in 1.22s. (Edit 2017-02-11, after compiler change)<br>
It should be much faster with a compiled language.<br>
<strong>Warning</strong> : It's my hardest problem.
Have fun ;-)</p>