<p>This problem is a higher constraints and generalized version of <a href="http://pl.spoj.com/problems/KWACIK/">KWACIK</a>&nbsp;(Polish) and <a href="../GRIDSUM2/">GRIDSUM2</a>.</p>
<p style="text-align: center;"><img title="Sample case for k=5, a=1, b=3 and n=8." src="../../../content/min_25:grid_5x5.png" alt="Sample case for k=5, a=1, b=3 and n=8." width="286" height="286"></p>
<p style="text-align: left;">&nbsp;</p>
<p>You are given a <strong><em>k</em></strong>x<strong><em>k</em></strong>&nbsp;grid. You can place an integer <em>m</em> (<strong><em>a</em></strong>&nbsp;��&nbsp;<em>m</em> ��&nbsp;<em><strong>b</strong></em>) in each cell.</p>
<p>How many ways are there to place integers in the cells such that the sum of each 2x2 subgrid is <em><strong>n</strong></em> ?</p>
<p>Since the answer might be very large, output it modulo <strong>479001600</strong> (= <strong>12!</strong>).</p>
<h3>Input</h3>
<p>The first line contains an integer <strong><em>T</em></strong>&nbsp;(1 �� <em><strong>T</strong></em> �� 10<sup>4</sup>), the number of test cases.</p>
<p>On each of the next <strong><em>T</em> </strong>lines, you are given four integers <strong><em>k</em></strong>,&nbsp;<em><strong>a</strong></em>, <strong><em>b</em></strong>&nbsp;and <em><strong>n</strong></em>.</p>
<p>(2 �� <strong><em>k</em></strong> �� 5,&nbsp;0 �� <strong><em>a</em></strong> �� <strong><em>b</em></strong> �� 5 * 10<sup>8</sup>, 0 �� <strong><em>n</em></strong> �� 2 * 10<sup>9</sup>)</p>
<h3>Output</h3>
<p>For each test case, output a single line containing the number of ways to place integers modulo <strong>479001600</strong>&nbsp;(=&nbsp;<strong>12!</strong>).</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>4
2 1 2 4
3 1 2 5
4 1 3 6
5 1 3 8
</pre>
<p><strong>Output:</strong></p>
<pre>1
8
74
1383
</pre>
<h3>Explanation</h3>
<p>There are 8 ways to place integers for <em><strong>k</strong></em>=3,&nbsp;<em><strong>a</strong></em>=1, <em><strong>b</strong></em>=2 and <strong><em>n</em></strong>=5.</p>
<pre>2 1 2 : 2 1 2 : 2 1 1 : 1 2 1 : 1 2 1 : 1 1 2 : 1 1 1 : 1 1 1
1 1 1 : 1 1 1 : 1 1 2 : 1 1 1 : 1 1 1 : 2 1 1 : 2 1 2 : 1 2 1
2 1 2 : 1 2 1 : 2 1 1 : 2 1 2 : 1 2 1 : 1 1 2 : 1 1 1 : 1 1 1
</pre>
<h3>Credit &amp; Special thanks</h3>
<ul>
<li><a href="../../../users/crucian/">Bartek</a>&nbsp;-&nbsp;the original problem author</li>
<li><a href="../../../users/cyclops/">Mitch Schwartz</a></li>
</ul>