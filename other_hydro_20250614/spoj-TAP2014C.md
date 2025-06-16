<p><strong>[The original version of this problem (in Spanish) can be found at <a title="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf" href="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf">http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf</a> ]</strong></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">One morning, when Cyrus Samsa woke from troubled dreams, he found himself lying on his bed, but not transformed into a monstrous insect. However, when he looked at the still starry sky, he found that the visual setting of cosmos showed four stars positioned as the vertices of a perfect parallelogram. Being a big geometry enthusiast, he called those four stars "constellation of the parallelogram".</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">A parallelogram is a four-sided polygon with its pairs of opposite sides being of identical length. Equivalently, a parallelogram is a convex quadrilateral whose diagonals intersect at their midpoints. The following figure illustrates both definitions, for a parallelogram with sides of lengths L and l, and diagonals of lengths D and d.</div>
<p>One morning, when Cyrus Samsa woke from troubled dreams, he found himself lying on his bed, but not transformed into a monstrous insect. However, when he looked up at the still starry sky, he found that the visual setting of the cosmos showed four stars positioned as the vertices of a perfect parallelogram. Being a big geometry enthusiast, he called those four stars "constellation of the parallelogram".</p>
<p>A parallelogram is a four-sided polygon with its pairs of opposite sides being of identical length. Equivalently, a parallelogram is a convex quadrilateral whose diagonals intersect at their midpoints. The following figure illustrates both definitions, for a parallelogram with sides of lengths <strong>L</strong> and <strong>l</strong>, and diagonals of lengths <strong>D</strong> and <strong>d</strong>.</p>
<p style="text-align: center;"><img title="Figure 1" src="../../content/fidels:TAP2014C1.png" alt="Figure 1"></p>
<p>Unfortunately, astronomers still do not agree on which were the stars that Cyrus was looking at. The problem is that on each image obtained of the sky's configuration, there are usually many sets comprising four stars that are the vertices of a parallelogram.</p>
<p>A starry sky is represented on an image as a set of points in the Cartesian plane, each of them corresponding to a star. The following figure shows three copies of the same image, each illustrating one of the three sets of four stars which are the vertices of a parallelogram, which are marked in the figure with solid lines.</p>
<p style="text-align: center;"><img title="Figure 2" src="../../content/fidels:TAP2014C2.png" alt="Figure 2"></p>
<p>Your task is to safeguard the good name of astronomers by calculating, given an image, the number of parallelograms contained in it.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>N</strong> indicating the number of stars on the image to be analyzed (<strong>4 ��&nbsp;N&nbsp;</strong><strong>��</strong><strong>&nbsp;1000</strong>).</p>
<p>The following <strong>N</strong> lines describe each of the stars on the image with two integers <strong>X<sub>i</sub></strong> and <strong>Y<sub>i</sub></strong>, indicating respectively the <strong>X</strong> and <strong>Y</strong> coordinates of the star on the Cartesian plane (<strong>-10<sup>8</sup>&nbsp;</strong><strong>��</strong><strong>&nbsp;X<sub>i</sub>, Y<sub>i</sub>&nbsp;</strong><strong>��</strong><strong>&nbsp;10<sup>8</sup></strong> for <strong>i = 1, 2, ..., N</strong>). You may assume that no two stars on the image are on the same position.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print a single line containing a single integer representing the number of sets of four points on the input image that are the vertices of a parallelogram.</p>
<p>&nbsp;</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">7
0 1
1 3
2 4
3 1
4 2
4 3
5 0</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">3</span></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">11
0 0
0 1
0 -1
1 0
1 1
1 -1
-1 0
-1 1
-1 -1
0 2
1 2</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">44</span></pre>
<h3>Example 3</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">4
0 0
0 1
0 2
0 3</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">0</span></pre>
<h3>Example 4</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">6
-100000000 100000000
100000000 -100000000
-100000000 -100000000
100000000 100000000
1 1
-1 -1</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">2</span></pre>