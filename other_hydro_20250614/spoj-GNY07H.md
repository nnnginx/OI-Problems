<p>We wish to tile a grid 4 units high and <i><b>N</b></i> units long with rectangles (dominoes) 2 units by one unit (in
either orientation). For example, the figure shows the five different ways that a grid 4 units high and 2
units wide may be tiled.

</p><p><img align="center" src="./22614/file/qAiSveu8.png">

</p><p>Write a program that takes as input the width, <i><b>W</b></i>, of the grid and outputs the number of different ways
to tile a 4-by-<i><b>W</b></i> grid.

</p><h3>Input</h3>
<p>The first line of input contains a single integer <i><b>N</b></i>, (1 ¡Ü <i><b>N</b></i> ¡Ü 1000) which is the number of datasets that
follow.
</p><p>Each dataset contains a single decimal integer, the width, <i><b>W</b></i>, of the grid for this problem instance.

</p><h3>Output</h3>
<p>For each problem instance, there is one line of output: The problem instance number as a decimal
integer (start counting at one), a single space and the number of tilings of a 4-by-<i><b>W</b></i> grid. The values
of <i><b>W</b></i> will be chosen so the count will fit in a 32-bit integer.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
2
3
7

<b>Output:</b>
1 5
2 11
3 781
</pre>