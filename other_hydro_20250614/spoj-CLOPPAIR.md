<p>You are given N points on a plane and your task is to find a pair of points with the smallest euclidean distance between them.</p>
<p>All points will be unique and there is only one pair with the smallest distance.</p>
<h3>Input</h3>
<p>First line of input will contain N (2&lt;=N&lt;=50000) and then N lines follow each line contains two integers giving the X and Y coordinate of the point. Absolute value of X,Y will be atmost 10^6.</p>
<h3>Output</h3>
<p>Output 3 numbers a b c, where a,b (a&lt;b) are the indexes (0 based) of the point pair in the input and c is the distance between them. Round c to 6 decimal digits.</p>
<p>See samples for more clarification.</p>
<p>&nbsp;</p>
<pre><strong>Input:</strong> <br>5 <br>0 0<br>0 1<br>100 45<br>2 3<br>9 9<br><strong><br>Output:</strong> <br>0 1 1.000000<br><pre><strong>Input:</strong> <br>5<br>0 0<br>-4 1<br>-7 -2<br>4 5<br>1 1<br><strong><br>Output:</strong> <br>0 4 1.414214<br></pre>
</pre>