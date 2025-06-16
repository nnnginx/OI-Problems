<p>Ankur, Anuja and Jyoti are planning to have party at some place. Their houses are located at different points in a rectangular grid of size M*N. They want to meet in minimum time and then party.</p>
<p>The M rows and N columns rectangular grid contains some impassable points (denoted by a #), however. So none of them wants to step over these points. They can only step over passable points (denoted by a .). They can also meet at some point outside the grid. You can assume that the points outside the grid are all passable. They cannot party on an impassable point and they have their house only on passable point. They can move either to North, South, East or West passable point from the current passable point and it takes 1 unit time to do so. Also they can wait at a passable point if they want to.</p>
<p>Find the minimum time of meeting.</p>
<p><strong>Note: Assume that they will always meet at some point.</strong></p>
<h3>Input</h3>
<p>First line gives T, the no. of test cases.</p>
<p>Each test case has two space separated integers M and N, the dimensions of the grid.</p>
<p>Next M lines contain N characters per line (no spaces). Characters can be either ¡°#¡± (impassable) or ¡°.¡± (passable) or ¡°1¡± (Ankur¡¯s house) or ¡°2¡± (Anuja¡¯s House) or ¡°3¡± (Jyoti¡¯s house). Each test case will have exactly 1 ¡°1¡±, exactly 1 ¡°2¡± and exactly 1 ¡°3¡±.</p>
<h3>Output</h3>
<p>Output T lines, each containing the required answer.</p>
<h3>Constraints</h3>
<p>1&lt;=T&lt;=10 <br> 1&lt;=M&lt;=200<br> 1&lt;=N&lt;=200</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 388px; width: 1px; height: 1px; overflow: hidden;">4 4</div>1
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 388px; width: 1px; height: 1px; overflow: hidden;">#...</div>4 4
#...
.2#.
..#3
1..#
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 388px; width: 1px; height: 1px; overflow: hidden;">.2#.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 388px; width: 1px; height: 1px; overflow: hidden;">..#3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 388px; width: 1px; height: 1px; overflow: hidden;">1..#</div><strong>Output:</strong>
4<span style="white-space: normal;">
</span></pre>