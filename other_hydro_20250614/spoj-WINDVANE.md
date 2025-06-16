<p><strong>Problem Statement:</strong></p>
<p>Wind vane is an instrument for showing the direction of the wind.</p>
<p style="text-align: center;">&nbsp;<img src="./24982/file/lGh2kACH.png" alt="" width="220" height="165"></p>
<p>Dream city is in the shape of a matrix of dimensions mxn. To monitor the direction of the wind in the city, wind vanes are placed in every unit cell of the city. According to the direction of the wind, these wind vanes turn themselves. Lets assume that there are only 4 directions North, East, West and South denoted by (¡®N¡¯,¡¯E¡¯,¡¯W¡¯,¡¯S¡¯). We know the initial direction of the wind vanes.</p>
<p>We denote the direction of change of wind by 0 (clockwise) and 1 (anti-clockwise)</p>
<p>Function ¡°Change(x1,y1,x2,y2,direction)¡±, changes the direction of the vanes in the sub-matrix (from x1,y1 to x2,y2) in the specified ¡®direction¡¯</p>
<p>(for example if the initial state of a cell is ¡®N¡¯ and the direction is clockwise, then the cell changes to ¡®E¡¯)</p>
<p>The ¡®Change¡¯ may occur any time. We need to know the direction of the wind at any unit cell at any instant.</p>
<p>Direction (x,y) should print the direction of the vane at the cell (x,y).</p>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p>The first line of the input consists two integers m and n - the dimentions of the city. Then follows the description of the matrix which denotes the direction of the vanes. The next line contains an integer c, the number of commands to process. Each command can be either of the format "C x1 y1 x2 y2 d" or "D x y".</p>
<p><strong>Output:</strong></p>
<p>Process the commands and print whenever necessary.</p>
<p>&nbsp;</p>
<p><strong>Input Constraints:</strong></p>
<p>1&lt;=m&lt;=1000</p>
<p>1&lt;=n&lt;=1000</p>
<p>each character in the matrix is one among {'N','E','W', and 'S'}</p>
<p>1&lt;=c&lt;=10000</p>
<p>1&lt;=x1,y1,x2,y2,x,y&lt;=1000</p>
<p>d= 0(clockwise) or 1(anti-clockwise)</p>
<p>x1&lt;=x2 y1&lt;=y2</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>5 5<br>ESWNE<br>NWWWN<br>EEESE<br>SSWSN<br>SNWEN<br>5<br>C 2 1 4 1 1<br>D 3 1<br>D 3 3<br>C 2 1 5 2 0<br>D 3 1</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>N</p>
<p>E</p>
<p>E</p>