<p>The city of Desrugenstein is a complete mess. Looking at the map, it seems organized, since it<br>was created in a square grid form, but there is no directions standard. Each corner says the directions<br>you can go from there (north, south, west, east). The mayor Daniel Snake is headstrong and lazy<br>enough to let everything as it is and forbid any change attempt. Unable to do much, the Master<br>Spiritual Counselor of Desrugenstein, Giordano Marfyn, asked you, Spiritual Counselor Level XVII of<br>Desrugenstein, lead programmer of Desrugenstein, to write a program to calculate the cost of going<br>from a corner (x, y) to another corner (z, w), considering the messy streets.</p>
<h3>Input</h3>
<p>Input file contains several test cases. First line of each test case contains an integer N (1 �� N �� 10) that<br>represents height and width of the grid that maps the city (a N x N grid). The input file ends with N = 0,<br>and it should not be processed. Each one of the next N lines represents a street of the city, starting from<br>the further north (N �C 1) until the further south. In each one of these lines there are 4*N integers, 4 for<br>each corner: A (north) B (south) C (west) D (east). Each one is 0 if it is not possible to go on the<br>respective direction, or 1 if it is possible.<br>After the city map, your program should read an integer P (1 �� P �� 100). Next P lines contain 4 integers<br>each, x0 y0 x1 y1 representing the question: ��What is the minimum cost to go from corner (x 0 , y0) to<br>corner (x1 , y1)?��. The cost to go from a corner to the nearest corner in any direction is 1.</p>
<h3>Output</h3>
<p>For each question, answer ��Impossible�� if there is no valid (respecting corners directions) path between<br>the corners, or the minimum cost, if there is(are) path(s). Print a blank line after each test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4<br>0 1 0 1 0 0 1 0 0 0 0 1 0 1 0 0<br>0 0 0 0 1 0 0 1 0 0 0 1 0 1 0 0<br>1 0 0 0 1 0 1 0 1 1 0 0 0 1 1 0<br>0 0 0 0 0 0 1 0 0 0 1 0 0 0 0 0<br>5<br>1 3 0 3<br>2 3 3 0<br>2 3 0 0<br>3 1 3 2<br>0 3 0 0<br>0

<strong>Output:</strong>
1<br>4<br>7<br>3<br>Impossible
</pre>