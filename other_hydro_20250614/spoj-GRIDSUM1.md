<p>This problem is a higher constraints version of <a href="http://pl.spoj.com/problems/KWACIK/">KWACIK</a>&nbsp;(Polish).</p>
<p style="text-align: center;"><img title="Sample case for a=1, b=3 and n=8." src="../../../content/min_25:grid_3x3.png" alt="Sample case for a=1, b=3 and n=8." width="312" height="312"></p>
<p style="text-align: left;">&nbsp;</p>
<p>You are given a 3x3 grid. You can place an integer <em>m</em> (<strong><em>a</em></strong>&nbsp;¡Ü&nbsp;<em>m</em> ¡Ü&nbsp;<em><strong>b</strong></em>) in each cell.</p>
<p>How many ways are there to place integers in the cells such that the sum of each 2x2 subgrid is <em><strong>n</strong></em> ?</p>
<h3>Input</h3>
<p>The first line contains an integer <strong><em>T</em></strong>&nbsp;(1 ¡Ü <em><strong>T</strong></em> ¡Ü 100), the number of test cases.</p>
<p>On each of the next <strong><em>T</em> </strong>lines, you are given three integers <em><strong>a</strong></em>, <strong><em>b</em></strong>&nbsp;and <em><strong>n</strong></em>. (0 ¡Ü <strong><em>a</em></strong> ¡Ü <strong><em>b</em></strong> ¡Ü 500, 0 ¡Ü <strong><em>n</em></strong> ¡Ü 2000)</p>
<h3>Output</h3>
<p>For each test case, output a single line containing the number of ways to place integers.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>1
1 2 5
</pre>
<p><strong>Output:</strong></p>
<pre>8</pre>
<h3>Explanation</h3>
<p>There are 8 ways to place integers for <em><strong>a</strong></em>=1, <em><strong>b</strong></em>=2 and <strong><em>n</em></strong>=5.</p>
<pre>2 1 2 : 2 1 2 : 2 1 1 : 1 2 1 : 1 2 1 : 1 1 2 : 1 1 1 : 1 1 1
1 1 1 : 1 1 1 : 1 1 2 : 1 1 1 : 1 1 1 : 2 1 1 : 2 1 2 : 1 2 1
2 1 2 : 1 2 1 : 2 1 1 : 2 1 2 : 1 2 1 : 1 1 2 : 1 1 1 : 1 1 1</pre>
<ul>
</ul>
<h3>Information</h3>
<p>- There are 7 input files.</p>
<p>- Changed the time limit of the input file #7 to 20 seconds and rejudged all submissions. (2014-10-17)</p>
<h3>Credit &amp; Special thanks</h3>
<ul>
<li><a href="../../../users/crucian/">Bartek</a>&nbsp;-&nbsp;the original problem author</li>
<li><a href="../../../users/cyclops/">Mitch Schwartz</a></li>
</ul>