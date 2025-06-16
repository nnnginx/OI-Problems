<p>Bob is a strategy game programming specialist. In his new city building game the gaming environment is as follows: a city is built up by areas, in which there are streets, trees, factories and buildings. There is still some space in the area that is unoccupied. The strategic task of his game is to win as much rent money from these free spaces. To win rent money you must erect buildings, that can only be rectangular, as long and wide as you can. Bob is trying to find a way to build the biggest possible building in each area. But he comes across some problems - he is not allowed to destroy already existing buildings, trees, factories and streets in the area he is building in.</p>
<p>Each area has its width and length. The area is divided into a grid of equal square units.The rent paid for each unit on which you're building stands is 3$.</p>
<p>Your task is to help Bob solve this problem. The whole city is divided into <b>K</b> areas. Each one of the areas is rectangular and has a different grid size with its own length <b>M</b> and width <b>N</b>. The existing occupied units are marked with the symbol <b>R</b>. The unoccupied units are marked with the symbol <b>F</b>.</p>

<h3>Input</h3>
<p>The first line of the input contains an integer <b>K</b> - determining the number of datasets. Next lines contain the area descriptions. One description is defined in the following way: The first line contains two integers-area length <b>M</b>&lt;=1000 and width <b>N</b>&lt;=1000, separated by a blank space. The next <b>M</b> lines contain <b>N</b> symbols that mark the reserved or free grid units,separated by a blank space. The symbols used are:</p>
<p><b>R</b> - reserved unit</p>
<p><b>F</b> - free unit</p>
<p>In the end of each area description there is a separating line.</p>

<h3>Output</h3>
<p>For each data set in the input print on a separate line, on the standard output, the integer that represents the profit obtained by erecting the largest building in the area encoded by the data set.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
5 6
R F F F F F
F F F F F F
R R R F F F
F F F F F F
F F F F F F

5 5
R R R R R
R R R R R
R R R R R
R R R R R
R R R R R

<b>Output:</b>
45
0
</pre>