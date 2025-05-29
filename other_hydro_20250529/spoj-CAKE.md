<p>Adolf wants to send a cake to Blue Mary to celebrate her birthday. The cake looks like a tower which has M floors, each floor is a cylinder. The i-th cylinder counted from downside to upside has a integer height h<sub>i</sub> and a integer radius r<sub>i</sub>. These numbers fulfill the following two conditions:</p>
<div>
<ul>
<li> h<sub>1</sub> &gt; h<sub>2</sub> &gt; h<sub>3</sub> &gt; ... &gt; h<sub>M</sub> </li>
<li> r<sub>1</sub> &gt; r<sub>2</sub> &gt; r<sub>3</sub> &gt; ... &gt; r<sub>M</sub></li>
</ul>
</div>
<p>Adolf is interested in minimising the area of the surface of the cake, except for the underside of the lowest cylinder. He needs your help because of his poor math knowledge.</p>
<h3>Input</h3>
<p>The very first line contains a integer number T. T test cases follow.</p>
<p>For each test case, the first line contains a single integer number N (N&lt;=10000), the second line contains a single integer number M (M&lt;=10). The cake must be made of M cylinders and its volume must be N*Pi (Pi = acos(-1.0)).</p>
<h3>Output</h3>
<p>For each test case, a single line containing a single integer S must be written to output. The required minimum area must be S*Pi.</p>
<h3>Example</h3>
<pre><strong><tt>Sample Input:</tt></strong>
1
100
2

<strong><tt>Sample Output:</tt></strong>
68
</pre>