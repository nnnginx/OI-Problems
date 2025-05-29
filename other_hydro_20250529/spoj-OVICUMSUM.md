<p>Given an array a<sub>0</sub> of size <strong>n</strong> (1 <strong><span style="text-decoration: underline;">&lt;</span></strong> n <strong><span style="text-decoration: underline;">&lt;</span></strong> 10<sup>5</sup>). Find the array a<sub>k</sub> modulo (<strong>7340033</strong>)</p>
<p>where a<sub>k</sub> = cumulative summation array of the array <strong>a</strong><sub>k-1</sub>.</p>
<p>&nbsp;</p>
<p>Means,</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>a</strong><sub>k</sub>[1] = <strong>a</strong><sub>k-1</sub>[1]</p>
<p>for i &gt; 1 , <strong>a</strong><sub>k</sub>[i] = <strong>a</strong><sub>k</sub>[i-1] + <strong>a</strong><sub>k-1</sub>[i]</p>
<p>&nbsp;</p>
<p>Given <strong>k</strong> (0 <span style="text-decoration: underline;">&lt;</span> k <span style="text-decoration: underline;">&lt;</span> <strong>10<sup>5</sup></strong>)</p>
<p>Can you find the array a<sub>k</sub> efficiently?</p>
<p>&nbsp;</p>
<p><strong>For example</strong>,</p>
<p>&nbsp;</p>
<p>If&nbsp; a<sub>0</sub> = {1, 2, 1, 3},</p>
<p>&nbsp;&nbsp;&nbsp; a<sub>1 </sub>&nbsp;= {1, 3, 4, 7}</p>
<p>&nbsp;&nbsp;&nbsp; a<sub>2</sub> = {1, 4, 8, 15}</p>
<p>&nbsp;&nbsp;&nbsp; a<sub>3</sub> = {1, 5, 13, 28}&nbsp;&nbsp;</p>
<h3>Input</h3>
<p>First line will contain two integer <strong>n</strong>, <strong>k</strong> (size of the array and <strong>k</strong> from the problem description)</p>
<p>&nbsp;</p>
<p>Following n positive integers separated by spaces denoting array a<sub>0</sub> .</p>
<p>All integers are smaller than 10<sup>5</sup>.</p>
<h3>Output</h3>
<p>Output n integers of the array <strong>a<sub>k</sub></strong> with spaces in between.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>4 2</p><p>1 2 1 3</p><strong>Output:</strong>
1 4 8 15</pre>