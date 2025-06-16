<p>On a faraway planet, strange plants with two stems can be found. Every plant on the planet can be described by three numbers: the x-coordinates of the stems L and R, and the height H at which the stems are connect. The image depicts a plant with L=2, R=5 and H=4.</p>
<p><img src="./22039/file/PuFJbnei.png" alt="" width="176" height="134"></p>
<p>Every day a new plant grows on the planet. The plant that grows on day 1 is of height 1, and every subsequent plant is one higher than the previous one.</p>
<p>When a stem of a new plant intersects the horizontal segment of another plant, a small flower grows (if one wasn't there already). If segments merely touch in a point, a flower will not grow there. The following images are a visualization of the first example.</p>
<p><img src="./22039/file/MOhD3hl7.png" alt="" width="176" height="134"> <img src="./22039/file/zBCmIMrh.png" alt="" width="176" height="134"> <img src="./22039/file/Ed9pvstP.png" alt="" width="176" height="134"> <img src="./22039/file/PrHuI5Qx.png" alt="" width="176" height="134"></p>
<p>Write a program that, given the coordinates of all plants, calculates the number of new flower every day.</p>
<h3>Input</h3>
<p>The first line contains an integer N (1 ¡Ü N ¡Ü 100 000), the number of days.</p>
<p>Each of the following N lines contains two integers L and R (1 ¡Ü L &lt; R ¡Ü 100 000), the coordinates of the stems of a plant.</p>
<h3>Output</h3>
<p>Output N lines, the number of new flowers after each plant grows.</p>
<h3>Example</h3>
<pre>Input
4
1 4
3 7
1 6
2 6

Output
0
1
1
2


Input
5
1 3
3 5
3 9
2 4
3 8

Output
0
0
0
3
2
</pre>