<p>You are given three triangle houses. Each house is presented by three points in the 2D coordination. Houses are not overlap but can share points on their border.</p>
<p>You stay at point (sx, sy) and want to reach (ex, ey) by a shortest path. Your path can not intersect with a house but you can go a long a house’s border. However, you can not “go through” the walls as follow (just an example, please use natural meaning):</p>
<p style="text-align: center;"><img src="../../../content/huy391992:houses" alt="" width="273" height="191"></p>
<p>You are to write a program to print the length of the shortest path.</p>
<p><br>Input<br>The input begins with T – number of test cases. For each test case:<br>• The first line of each test case consists of sx, sy, ex, ey.<br>• In next three lines, each line consists of 6 numbers x1, y1, x2, y2, x3, y3 denote<br>coordinates of a house.</p>
<p><br>Output<br>For each test case, print the length of the shortest path with exactly 5 precision digits.</p>
<p><br>Limits<br>T &lt;= 20<br>The absolute values of coordinates are less than 1000.</p>
<p><br>Sample input<br>1<br>0 0 3 0<br>1 0 2 0 1 1<br>2 0 2 -1 3 -1<br>2 1 3 1 2 2</p>
<p><br>Sample output<br>3.65028</p>