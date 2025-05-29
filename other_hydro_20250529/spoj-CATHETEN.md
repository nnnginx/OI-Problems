<p>For any integer <strong><em>n</em></strong>,
we define <strong><em>F</em>(<em>n</em>)</strong> as the number of ways
in which <strong><em>n</em></strong> can be the cathetus (leg) of a Pythagorean triangle.<br>
For example, there is exactly four Pythagorean triangles with 15 as a length for a cathetus.</p>

<p><img title="catheten" src="../../content/francky:catheten" alt="catheten"></p>

<p>
(8 <strong>15</strong> 17),
(<strong>15</strong> 20 25),
(<strong>15</strong> 36 39),
(<strong>15</strong> 112 113)
</p>
<p>
Thus <strong><em>F</em>(15) = 4</strong>.
</p>

<h3>Input</h3>

<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.</p>

<p>Each of the next <strong><em>T</em></strong> lines contains
 a single integer <strong><em>n</em></strong>.</p>

<h3>Output</h3>
<p>For each test case, print <strong><em>F</em>(<em>n</em>)</strong> on a single line.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
5
10
15
</pre>
<pre><strong>Output:</strong>
1
1
4
</pre>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 10^5
0 &lt; n &lt; 10^9
</pre>
<p>For your information, my C code ran in 0.08s, whereas my python3 one ran in 0.90s. (Edit 2017-02-11, after compiler changes)</p>