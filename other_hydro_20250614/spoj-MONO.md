<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Mirko soon realised that number sequences are not the best career choice, and went right back to lettertable</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">business.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Mirko¡¯s table has R rows and C columns and consists of lowercase letters.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each cell of the table is a square of equal size. We assign coordinates to vertices of those squares, so</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">that upper-left corner of the table has coordinates (0, 0), upper-right (C,0), lower-left (0, R), and lowerright</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">(C, R).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">We say that polygon within the table is monoliteral if the following holds:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1. its vertices are from the described set of cell-square vertices,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2. its edges are parallel to coordinate axes,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3. all letters inside the polygon are equal.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">A simple polygon for which first two conditions are true (third one may or may not be true) is given.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Mirko would like to know the number of monoliteral polygons that can be obtained by moving the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">given one up, down, left, or right or any combination thereof, but not rotating.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">INPUT</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line of input contains two space seperated integers R and C (1 ¡Ü R, C ¡Ü 500).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each of the next R lines contains exactly C lowercase letters, this is Mirko¡¯s table.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The following line contains integer V (4 ¡Ü V ¡Ü 500), number of vertices of given polygon.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each of the next V lines contains two integers X, Y (0 ¡Ü X ¡Ü C, 0 ¡Ü Y ¡Ü R). These are the coordinates</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">of the vertices of the given polygon. Vertices are given in clockwise order.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The given polygon will satisfy conditions 1 and 2 from above.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">OUTPUT</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">In the first and only line of output, print expected number of polygons.</div>
<p>Mirko soon realised that number sequences are not the best career choice, and went right back to lettertable business.</p>
<p>Mirko¡¯s table has R rows and C columns and consists of lowercase letters.</p>
<p>Each cell of the table is a square of equal size. We assign coordinates to vertices of those squares, so&nbsp;that upper-left corner of the table has coordinates (0, 0), upper-right (C,0), lower-left (0, R), and lowerright&nbsp;(C, R).</p>
<p>We say that polygon within the table is monoliteral if the following holds:</p>
<p>1. its vertices are from the described set of cell-square vertices,</p>
<p>2. its edges are parallel to coordinate axes,</p>
<p>3. all letters inside the polygon are equal.</p>
<p>A simple polygon for which first two conditions are true (third one may or may not be true) is given.</p>
<p>Mirko would like to know the number of monoliteral polygons that can be obtained by moving the&nbsp;given one up, down, left, or right or any combination thereof, but not rotating.</p>
<p><strong>INPUT</strong></p>
<p>The first line of input contains two space seperated integers R and C (1 ¡Ü R, C ¡Ü 500).</p>
<p>Each of the next R lines contains exactly C lowercase letters, this is Mirko¡¯s table.</p>
<p>The following line contains integer V (4 ¡Ü V ¡Ü 500), number of vertices of given polygon.</p>
<p>Each of the next V lines contains two integers X, Y (0 ¡Ü X ¡Ü C, 0 ¡Ü Y ¡Ü R). These are the coordinates</p>
<p>of the vertices of the given polygon. Vertices are given in clockwise order.</p>
<p>The given polygon will satisfy conditions 1 and 2 from above.</p>
<p><strong>OUTPUT</strong></p>
<p>In the first and only line of output, print expected number of polygons.</p>
<p style="text-align: center;"><span style="font-size: medium;"><strong>Example</strong></span></p>
<p>&nbsp;</p>
<p><strong>input</strong></p>
<p>3 3</p>
<p>aaa</p>
<p>aaa</p>
<p>aaa</p>
<p>4</p>
<p>2 0</p>
<p>2 2</p>
<p>0 2</p>
<p>0 0</p>
<p>&nbsp;</p>
<p><strong>output</strong></p>
<p>4</p>
<p>&nbsp;</p>
<p><strong>input</strong></p>
<p>3 3</p>
<p>aaa</p>
<p>aba</p>
<p>aaa</p>
<p>4</p>
<p>2 0</p>
<p>2 2</p>
<p>0 2</p>
<p>0 0</p>
<p>&nbsp;</p>
<p><strong>output</strong></p>
<p>0</p>
<p>&nbsp;</p>
<p><strong>input</strong></p>
<p>5 4</p>
<p>xyyx</p>
<p>xyyy</p>
<p>xxyy</p>
<p>xxxx</p>
<p>xxxx</p>
<p>8</p>
<p>1 3</p>
<p>1 2</p>
<p>0 2</p>
<p>0 0</p>
<p>2 0</p>
<p>2 1</p>
<p>3 1</p>
<p>3 3</p>
<p><strong>output</strong></p>
<p>2</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>