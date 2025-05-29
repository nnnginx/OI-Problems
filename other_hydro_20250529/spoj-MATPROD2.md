<p><strong>[Note: <a title="Symmetric Matrix" href="../MATPROD/">Symmetric Matrix</a> is an easier version of this problem; you should try to solve it before this one.]</strong></p>
<p>You are given an&nbsp;<strong>N&nbsp;</strong>x&nbsp;<strong>N</strong>&nbsp;matrix&nbsp;<strong>m<sub>ij</sub>&nbsp;</strong>such that&nbsp;<strong>m<sub>ij</sub>&nbsp;== m<sub>ji</sub>&nbsp;</strong>for&nbsp;<strong>i, j = 1, ..., N</strong>. We would like to compute the value of</p>
<p style="text-align: center;"><img src="../../content/fidels:MATPROD.png" alt="" width="300" height="77"></p>
<p>Note that in the above expression we are going over&nbsp;<strong>K</strong>&nbsp;indices&nbsp;<strong>i<sub>1</sub>, ..., i<sub>K</sub></strong>&nbsp;that run over the values&nbsp;<strong>1, ..., N</strong>, while summing over the product of all the&nbsp;<strong>K*(K-1)/2&nbsp;</strong>possible matrix elements that we can form with these indices.</p>
<h3>Input</h3>
<p>The first line of the input contains two integers&nbsp;<strong>N</strong>&nbsp;and&nbsp;<strong>K</strong>&nbsp;(<strong>2 ¡Ü N ¡Ü 100</strong>&nbsp;and&nbsp;<strong>2 ¡Ü K ¡Ü 10</strong>), representing the number of rows and columns of the matrix&nbsp;<strong>m<sub>ij</sub>&nbsp;</strong>and the number of sums in the formula above, respectively. The following&nbsp;<strong>N</strong>&nbsp;lines contain&nbsp;<strong>N</strong>&nbsp;integers each, being the&nbsp;<strong>j</strong>-th&nbsp;number in the&nbsp;<strong>i</strong>-th line the value of&nbsp;<strong><strong>m</strong><sub>ij</sub></strong>&nbsp;(<strong>-10&nbsp; ¡Ü m<sub>ij</sub>&nbsp;¡Ü 10</strong>&nbsp;and&nbsp;<strong>m<sub>ij</sub>&nbsp;== m<sub>ji</sub></strong>&nbsp;for&nbsp;<strong>i, j = 1, ..., N</strong>).</p>
<h3>Output</h3>
<p>Print a single line with the result of the calculation. Because this number can be very big, output its remainder modulo division by<strong>1000000007&nbsp;</strong>(<strong>==&nbsp;10<sup>9</sup>+7</strong>).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 208px; width: 1px; height: 1px; overflow: hidden;">4 5</div><span style="font-family: 'courier new', courier;">4 5
-4 -3 -4 2
-3 -6 1 -8
-4 1 -10 -6
2 -8 -6 0
</span>
<strong>Output:</strong>
308822466</pre>