<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Hogwarts is under attack by the Dark Lord, He-Who-Must-Not-Be-Named. To protect the students, Harry Potter must cast protective spells so that those who are protected by the spells cannot be attacked by the Dark Lord.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Harry has asked all the students to gather on the vast quidditch sports field so that he can cast his spells. &nbsp;The students are standing in a 2D plane at all grid points - these are the points (x,y) such that both x and y are integers (positive, negative or 0). Harry's spell can take the shapes of triangle, circle or square, and all who fall within that shape (including its boundaries) are protected.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Given the types of spells and the details regarding where Harry casts the spell, output the number of people saved by Harry's spells.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains the number of test cases T. T test cases follow.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each case contains an integer N on the first line, denoting the number of spells Harry casts. N lines follow, each containing the description of a spell.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">If the ith spell is a triangle, then the line will be of the form "T x1 y1 x2 y2 x3 y3". Here, (x1,y1), (x2,y2) and (x3,y3) are the coordinates of the vertices of the triangle.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">If the ith spell is a circle, then the line will be of the form "C x y r". Here, (x,y) is the center and r is the radius of the circle.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">If the ith spell is a square, then the line will be of the form "S x y l". Here, (x,y) denotes the coordinates of the bottom-left corner of the square (the corner having the lowest x and y values) and l is the length of each side.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output T lines, one for each test case, denoting the number of people Harry can save.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">All numbers in the input are integers between 1 and 50, inclusive.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The areas of all geometric figures will be &gt; 0.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Time Limit: 3 s</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Memory Limit: 32 MBytes</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">C 5 5 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">S 3 3 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">T 1 1 1 3 3 1&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">C 10 10 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">S 9 8 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">T 7 9 10 8 8 10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">13</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">25</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">34</div>
<p>&nbsp;</p>
<p>Hogwarts is under attack by the Dark Lord, He-Who-Must-Not-Be-Named. To protect the students, Harry Potter must cast protective spells so that those who are protected by the spells cannot be attacked by the Dark Lord.</p>
<p>Harry has asked all the students to gather on the vast quidditch sports field so that he can cast his spells. &nbsp;The students are standing in a 2D plane at all grid points - these are the points (x,y) such that both x and y are integers (positive, negative or 0). Harry's spell can take the shapes of triangle, circle or square, and all who fall within that shape (including its boundaries) are protected.</p>
<p>Given the types of spells and the details regarding where Harry casts the spell, output the number of people saved by Harry's spells.</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains the number of test cases T. T test cases follow.</p>
<p>Each case contains an integer N on the first line, denoting the number of spells Harry casts. N lines follow, each containing the description of a spell.</p>
<p>If the ith spell is a triangle, then the line will be of the form "T x1 y1 x2 y2 x3 y3". Here, (x1,y1), (x2,y2) and (x3,y3) are the coordinates of the vertices of the triangle.</p>
<p>If the ith spell is a circle, then the line will be of the form "C x y r". Here, (x,y) is the center and r is the radius of the circle.</p>
<p>If the ith spell is a square, then the line will be of the form "S x y l". Here, (x,y) denotes the coordinates of the bottom-left corner of the square (the corner having the lowest x and y values) and l is the length of each side.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>Output T lines, one for each test case, denoting the number of people Harry can save.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>All numbers in the input are integers between 1 and 50, inclusive.</p>
<p>The areas of all geometric figures will be &gt; 0.</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>4</p>
<p>1</p>
<p>C 5 5 2</p>
<p>1</p>
<p>S 3 3 4</p>
<p>1</p>
<p>T 1 1 1 3 3 1&nbsp;</p>
<p>3</p>
<p>C 10 10 3</p>
<p>S 9 8 4</p>
<p>T 7 9 10 8 8 10</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>13</p>
<p>25</p>
<p>6</p>
<p>34</p>
<p>&nbsp;</p>
<p>&nbsp;</p>