<p>Â&nbsp; Â&nbsp; Minh has a box of pencils. The box is a rectangle of size M ĂN, where position (i, j) has a pencil Â&nbsp;with a length of exactly i Ă N + j (0 â¤ i â¤ M-1, 0 â¤ j â¤ N-1). Note that position (0, 0) does not have any pencil hence having a length of 0.</p>
<p>Â&nbsp; Â&nbsp; He wonders if he could select a sub-rectangle of the box and join all the pencils within that sub-rectangle together, to get a new long pencil that has a specific length L that he wants.</p>
<p>Â&nbsp; Â&nbsp; Your task is to find a sub-rectangle of the box in which the total length of the contained pencils is L and return the area of that the sub-rectangle. If there are multiple solutions, return the smallest Â&nbsp;possible area. If thereâs no such sub-rectangle, return -1.</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Minh has a box of pencils. The box is a rectangle of size M ĂN, where position (i, j) has a pencilÂ&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">with a length of exactly i Ă N + j (0 â¤ i â¤ M-1, 0 â¤ j â¤ N-1). Note that position (0, 0) does not haveÂ&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">any pencil hence having a length of 0.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">He wonders if he could select a sub-rectangle of the box and join all the pencils within that sub-</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">rectangle together, to get a new long pencil that has a specific length L that he wants.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Your task is to find a sub-rectangle of the box in which the total length of the contained pencilsÂ&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">is L and return the area of that the sub-rectangle. If there are multiple solutions, return the smallestÂ&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">possible area. If thereâs no s</div>
<h3>Input</h3>
<p>The input file consists of several datasets. The first line of the input file contains the number of</p>
<p>datasets which is a positive integer and is not greater than 150. The following lines describe theÂ&nbsp;</p>
<p>datasets.</p>
<p>Â&nbsp; Â&nbsp; Each dataset contains three space-separated numbers M, N and L (1 â¤ M, N â¤ 10^6,Â&nbsp;1 â¤ L â¤ 10^12) written in one line.</p>
<h3>Output</h3>
<p>Â&nbsp; Â&nbsp;For each dataset, write in one line the smallest possible area of the sub-rectangle in which the total sum of pencil lengths is L. Write in one line -1 if there is no such sub-rectangle.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
2 3 8
2 2 7</pre>
<pre><strong>Output:</strong>
4
-1</pre>