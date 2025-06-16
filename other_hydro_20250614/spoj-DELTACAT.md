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

<p>Geometrically, it is the study of right triangles for which the difference of the
catheti are equal to <strong><em>d</em></strong>.</p>

<h3>Input</h3>

<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.</p>

<p>Each of the next <strong><em>T</em></strong> lines contains
 three integers <strong><em>n, d, m</em></strong>.</p>

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
3 21 1000
9 119 11
</pre>
<pre><strong>Output:</strong>
3 4 5
63 84 105
5 3 1
</pre>

<h3>Explanations</h3>
<p>For the first case, the first solution is <strong>(3, 4, 5)</strong>, as 4 - 3 = 1.</p>
<p>For the second case, the firsts solutions are:<br>
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
<pre>0 &lt; T &lt; 10^5
0 &lt; n &lt; 10^7
0 &lt; d &lt; 10^8
1 &lt; m &lt; 10^9
</pre>
<p><strong><em>n, d, m</em></strong> : Uniform randomly chosen in their range.</p>
<p>Constraints allow some interpreted languages to get AC, but it could be hard.<br>
For your information, I have two distinct solutions.<br>
My first python3 code get AC under 17s.
My second python3 code get AC under 8s.<br>
(Timing updated, 2017-02-11 ; after compiler changes)<br>
With a compiled language, it should be at least 20¡Á faster. Have fun ;-)</p>