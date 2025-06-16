<p><strong>[NOTE: A harder version of this problem is <a title="Symmetric Matrix 2" href="../MATPROD2/">Symmetric Matrix 2</a>; you may want to try it once you solve this one.]</strong></p>
<p>You are given an <strong>N&nbsp;</strong>x&nbsp;<strong>N</strong>&nbsp;matrix <strong>m<sub>ij</sub>&nbsp;</strong>such that <strong>m<sub>ij</sub>&nbsp;== m<sub>ji</sub>&nbsp;</strong>for <strong>i, j = 1, ..., N</strong>. We would like to compute the value of</p>
<p style="text-align: center;"><img src="../../content/fidels:MATPROD.png" alt="" width="300" height="77"></p>
<p style="text-align: left;">Note that in the above expression we are going over <strong>K</strong>&nbsp;indices <strong>i<sub>1</sub>, ..., i<sub>K</sub></strong>&nbsp;that run over the values <strong>1, ..., N</strong>, while summing over the product of all the <strong>K*(K-1)/2&nbsp;</strong>possible matrix elements that we can form with these indices.</p>
<h3>Input</h3>
<p>The first line of the input contains two integers <strong>N</strong> and <strong>K</strong> (<strong>2 ¡Ü N ¡Ü 100</strong> and <strong>2 ¡Ü K ¡Ü 5</strong>), representing the number of rows and columns of the matrix <strong>m<sub>ij</sub>&nbsp;</strong>and the number of sums in the formula above, respectively. The following <strong>N</strong> lines contain <strong>N</strong>&nbsp;integers each, being the <strong>j</strong>-th&nbsp;number in the <strong>i</strong>-th line the value of <strong><strong>m</strong><sub>ij</sub></strong>&nbsp;(<strong>-10&nbsp; ¡Ü m<sub>ij</sub> ¡Ü 10</strong> and <strong>m<sub>ij</sub>&nbsp;== m<sub>ji</sub></strong> for <strong>i, j = 1, ..., N</strong>).</p>
<h3>Output</h3>
<p>Print a single line with the result of the calculation. Because this number can be very big, output its remainder modulo division by <strong>1000000007 </strong>(<strong>==&nbsp;10<sup>9</sup>+7</strong>).</p>
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