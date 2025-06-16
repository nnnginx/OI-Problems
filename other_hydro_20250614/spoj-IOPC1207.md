<p align="justify">The latest attraction for Techkriti 2112 is is a huge display of genetically modified plants. The arrangement consists of a cuboidal box of size N<sub>x</sub> ¡Á N<sub>y</sub> ¡Á N<sub>z</sub> made of unit cubes. Each unit cube is identified using (x,y,z) coordinates - x ranges from 0 to N<sub>x</sub>-1 and so on - and contains a plant genetically modified to show fluorescence. The natural colour of the plants is green. However, on exposing a plant to laser light, it changes colour to red. What is more interesting is that on exposing a red plant to laser light again, it changes back to green and this continues.</p>
<p align="justify">The organisers have realised that they can use the display to make many coloured patterns. They have with them a laser light sheet which they can place along an axis and move in one direction, exposing many plants to light at once. For example, if the plane of the light sheet is kept as the y axis and it is moved from a to b, every plant with the y coordinate between a and b inclusive will turn from green to red or red to green. Every time the laser is operated, it is only the plants with one specific coordinate in a certain range which are affected.</p>
<p align="justify">You are told that initially all plants were green. Given the sequence of exposing plants to laser light, your task is to find the number of red coloured plants in certain cuboidal subregions of the display</p>
<h3>Input</h3>
<p align="justify">The first line of the input contains T, the number of test cases (T ¡Ü 10). Following this are the descriptions of the T test cases. The description of each test case starts with a line containing four space separated integers : N<sub>x</sub>, N<sub>y</sub>, N<sub>z</sub> and Q (1 ¡Ü N<sub>x</sub>,N<sub>y</sub>,N<sub>z</sub> ¡Ü 100000; Q ¡Ü 5000). The first three are the extents of the display in the three dimensions while Q is the number of queries which are to follow. Following this are Q lines, each describing a query. A query will be of one of the following forms :</p>
<ul>
<li>0 i j : expose all plants with x coordinates i ¡Ü x ¡Ü j to laser light</li>
<li>1 i j : expose all plants with y coordinates i ¡Ü y ¡Ü j to laser light</li>
<li>2 i j : expose all plants with z coordinates i ¡Ü z ¡Ü j to laser light</li>
<li>3 x<sub>1</sub> y<sub>1</sub> z<sub>1</sub> x<sub>2</sub> y<sub>2</sub> z<sub>2</sub> : Report the number of red plants in the cuboidal region with (x<sub>1</sub>,y<sub>1</sub>,z<sub>1</sub>) and (x<sub>2</sub>,y<sub>2</sub>,z<sub>2</sub>) as diagonally opposite cells - ie, all red plants with x<sub>1</sub> ¡Ü x ¡Ü x<sub>2</sub>, y<sub>1</sub> ¡Ü y ¡Ü y<sub>2</sub> and  z<sub>1</sub> ¡Ü z ¡Ü z<sub>2</sub></li>
</ul>
<p>&nbsp;</p>
<p align="justify">All individual coordinates will be valid - ie, every x coordinate will be such that 0 ¡Ü x ¡Ü N<sub>x</sub>-1  and so on. Also, i ¡Ü j; x<sub>1</sub> ¡Ü x<sub>2</sub>; y<sub>1</sub> ¡Ü y<sub>2</sub> and z<sub>1</sub> ¡Ü z<sub>2</sub></p>
<h3>Output</h3>
<p align="justify">For every query of the form 3 x<sub>1</sub> y<sub>1</sub> z<sub>1</sub> x<sub>2</sub> y<sub>2</sub> z<sub>2</sub> in the input, output the number of red plants with coordinates constrained by x<sub>1</sub> ¡Ü x ¡Ü x<sub>2</sub>, y<sub>1</sub> ¡Ü y ¡Ü y<sub>2</sub> and  z<sub>1</sub> ¡Ü z ¡Ü z<sub>2</sub></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
3 4 5 5
0 1 2
1 2 3
3 0 0 0 1 2 3
2 3 4
3 1 1 1 2 2 2

<strong>Output:</strong>
12
4
</pre>