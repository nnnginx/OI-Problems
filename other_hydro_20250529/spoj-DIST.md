<p>You are given the coordinates of N cities (xi,yi). Each city also has a  popularity value, pi. You have to place a new city (x,y) such that the  sum of distances of this new point from all the other given points is  minimized. <br> Distance of the new point from a given city i is given by : <br> d = |xi - x| ^ pi + | yi - y | ^ pi</p>
<h3>Input</h3>
<p>There are multiple test cases. <br> First line contains the number of testcases. <br> Each testcases starts with the number N, the number of points. <br> This is followed by the descriptions of each in the format <br> xi yi pi <br> The input consists of only integers</p>
<h3>Output</h3>
<p>For each testcase, output the minimum distance obtained, with exactly 3 digits after the decimal point.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1 <br>3 <br>1 2 0 <br>4 5 1 <br>2 4 2<br><strong>Output:</strong>
4.500<br><br></pre>
<h3>Constraints</h3>
<p>No. of testcases &lt;= 10 <br> N &lt;= 10^5 <br> |xi,yi| &lt;= 1000 <br> 0 &lt;= pi &lt;= 3</p>