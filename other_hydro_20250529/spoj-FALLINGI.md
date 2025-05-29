<p>Imagine disks of ice falling, one at a time, into a box, each ending
up at the lowest point it can reach without overlapping or moving
previous disks.  Each disk then freezes into place, so it cannot
be moved by later disks.  Your job is to find the
overall height of the final combination of disks.</p>

<p>So that the answer is unique, assume that any disk reaching the
bottom of the box rolls as far to the left as possible.  Also the
data is chosen so there will be a unique lowest position for any disk
that does not reach the bottom.  The data is also such that there
are no "perfect fits":  each disk that lands will be in contact
with only two other points, on previous circles or the sides of the
box.  The illustrations above show white filled disks labeled with
the order in which they fall into their boxes.  The gray circle in
the fourth illustration is not intended to be a disk that fell in.
 The gray disk is included to demonstrate a point:  the gray
disk is the same size as disk 2, so there is <span style="font-style: italic;">space</span> 
for disk 2 on the very bottom of its box, but disk 2 cannot <span style="font-style: italic;">reach</span> 
that position by falling from the top.  It gets caught on disk 1 and the side of the box.  

</p>

<p>One way to find the top
intersection point of two intersecting circles is as follows.
Suppose circle 1 has center (x1, y1) and radius r1, and suppose circle 2 has center (x2, y2),
and radius r2. Also assume that circle 1 is to the left of circle 2, i.e., x1 &lt; x2. Let</p>

<p>dx = x2 - x1,<br>
dy = y2 - y1,<br>
D = sqrt(dx*dx + dy*dy),<br>
E = (r1*r1 - r2*r2 + D*D)/(2*D),<br>
F = sqrt(r1*r1 - E*E);</p>
<p>then the upper intersection point is (x1 + (E*dx - F*dy)/D, y1 + (F*dx + E*dy)/D).</p>

<br>
<p>
</p><center><img src="/content/zukow:FALLINGI.png" alt="subir imagenes" border="0"></center>
<br>

<h3>Input</h3>
<p>The input consists of one or more data
sets, followed by a line containing only 0 that signals the end of the input. Each data set is on
a line by itself and contains a sequence of three or more blank-separated
positive integers, in the format <span style="font-style: italic;">w</span>, 

<span style="font-style: italic;">n</span>, 
<span style="font-style: italic;">d</span><sub style="font-style: italic;">1</sub>,
<span style="font-style: italic;"> d</span><sub style="font-style: italic;">2</sub>, 
<span style="font-style: italic;">d</span><sub style="font-style: italic;">3</sub>, ..., 
<span style="font-style: italic;">d</span><sub style="font-style: italic;">n</sub>, where 
<span style="font-style: italic;">w</span> is the width of the box, 

<span style="font-style: italic;">n</span> is the number of disks, and the remaining numbers are 
the diameters of the disks, in the order in which they fall into the box.  
You can assume that <span style="font-style: italic;">w</span> &lt; 100, 
that <span style="font-style: italic;">n</span> &lt; 10, and that each diameter is less than 
<span style="font-style: italic;">w</span>.
</p>


<h3>Output</h3>
<p> For each data set, output a single line
containing the height of the pile of disks, rounded to two places
beyond the decimal point.</p>

<p>The example data matches the illustrations above.</p>


<h3>Example</h3>

<pre><b>Input:</b>
10 3 5 2 3
8 2 5 5
11 3 10 2 4
9 3 4 4 6
10 6 5 4 6 3 5 2
0 

<b>Output:</b>
5.00
9.00
12.99
9.58
14.19

</pre>