<p>Iron man is hovering over enemy territories. He comes across their weapons warehouse. The weapons are stored in<strong> N </strong>rectangular  boxes. No two boxes share edges. Boxes may be located inside other  boxes but no two boxes will partially overlap each other. Iron man can  destroy a box by sending a magnetic pulse with power equal to area of  the box (irrespective of the height of the box). This pulse will destroy  anything present inside the box. Since Iron man is running low on  power, he conveys the 2-D coordinates of all the boxes (as seen from the  top view) to Jarvis(artificial intelligence) to calculate the minimum  total power of the pulses that will be used to destroy all the boxes. Help Jarvis in determining the total effective area of the weapon  warehouse to which the beam needs to be directed to destroy all the  boxes.</p>
<h3>Input</h3>
<p>The first line of the input contains an integer <strong>N</strong> denoting the number of rectangular boxes. <strong>N</strong> lines follow. Each following line contains 4 integers- <strong>x_1, y_1, x_2, y_2</strong> where coordinates <strong>(x_1,y_1)</strong> and <strong>(x_2,y_2)</strong> uniquely identify a rectangular box.</p>
<ul>
<li><strong>1</strong> ¡Ü <strong>N</strong> ¡Ü <strong>10<sup>5</sup></strong></li>
<li><strong>-10<sup>8</sup></strong> ¡Ü <strong>x_1, y_1, x_2, y_2</strong> ¡Ü <strong>10<sup>8</sup></strong></li>
</ul>
<h3>Output</h3>
<p>Print the total effective area to be destroyed.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
0 0 2 2
-1 -1 4 4
5 5 8 8

<strong>Output:</strong>
34</pre>
<h3>Explanation</h3>
<p>In the given test case, first box lies completely inside the second box so we need not to consider that box in calculating the total effective  area. Therefore the answer will simply be the sum of areas of the second and third boxes that is 25+9=34</p>