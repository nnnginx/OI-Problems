<p>When Natalia is not having fun studying Computing Science in Santiago de los Caballeros, she opens up her bag and pulls out an iPad she won at a Programming Olympiad to play a classical maze game.</p>
<p>The maze is a rectangular figure of M rows and N columns. Open areas are represented by a 'O' while closed areas are represented by a '*'. An area is just a 1x1 block inside the maze. There's an entrance area marked by a '$' and a destination area marked by a '#'. Please note that both the entrance and destination are also open areas.&nbsp;</p>
<p>Once Natalia is located inside an open area, she can decide to move to either cardinal direction (north, south, east or west). In other words, if Natalia is located at (x,y), she can move to either&nbsp;(x + 1, y),&nbsp;(x - 1, y), &nbsp;(x, y + 1) or (x, y - 1). Of course, she can't move inside a closed area.</p>
<p>Given a rectangular maze as described above, output the minimum number of steps necessary to reach the final position from the starting area, if it is possible. If not, output '-1'.</p>
<h3>Input</h3>
<p>The input contains many lines. The first line contains an integer T (1 �� T �� 100), the number of test cases. For each test case there's a first line that contains two space separated integers M and N (1 �� M �� 100), (2 �� N �� 100), the dimensions of the maze. The line is followed by M lines. Each of these lines contain a string of N characters. The position at index j of the ith string represents the marker of the i,j area. It can be either an open marker ('O'), a closed marker ('*'), the unique entrance marker ('$') or the unique destination marker ('#').&nbsp;</p>
<h3>Output</h3>
<p>For each test case output the minimum number of steps necessary to reach the final position from the entrance position. If it is impossible to reach the final position, output -1.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">$OO</div>2
3 3
$OO
***
OO#
3 3
$*#
O*O
OOO
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">***</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">O#</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 3</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">$*#</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">O*O</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">OOO2
3 3
$OO
***
OO#
3 3
$*#
O*O
</div></pre>
<pre><strong>Output:</strong>
<p>-1<br>6</p></pre>