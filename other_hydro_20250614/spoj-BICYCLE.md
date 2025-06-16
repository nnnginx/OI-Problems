<p>Peter likes to go to school by bicycle. But going by bicycle on sidewalks is forbidden and going along roads is dangerous. That's why Peter travels only along special bicycle lanes. Fortunately Peter's home and school are in the immediate proximity of such paths. In the city where Peter lives there are only two bycycle lanes. Both lanes have the form of a circle. At the points where they cross it is possible to move from one path to the other. Peter knows the point where he enters the road and the point at which it is necessary to leave to enter the school. Peter is interested in the question: "What is the minimal distance he needs to cover along the lanes to get to school?"
</p>

<h3>Input</h3>
<p><i>t</i> ¨C the number of test cases [<i>t</i>&lt;=100],
then <i>t</i> test cases follow. <br>
The first 2 lines of each test case contain the description of the bicycle lanes:<br>
<i>x1 y1 r1</i> - 3 integers (<i>x1, y1</i> - coordinates of the center of the 1st circle, <i>r1</i> - radius of 1st circle)<br>
<i>x2 y2 r2</i> - 3 integers (<i>x2, y2</i> - coordinates of the center of the 2nd circle, <i>r2</i> - radius of 2nd circle)<br> 
-200 &lt;= <i>x1, x2, y1, y2</i> &lt;= 200<br>
0 &lt;= <i>r1, r2</i> &lt;= 200<br>
Next 2 lines contain the coordinates of Peter's home and school:<br>
<i>px1, py1</i> - 2 real numbers<br>
<i>px2, py2</i> - 2 real numbers</p><p>
You may assume that this points lie on the circle with high accuracy (10<sup>-8</sup>). Both points may lie on the same circle.

</p><h3>Output</h3>
<p>For each test case output the minimum distance that Peter needs to go from home to get to school. The precision of the answer must be under 0.0001. If it's impossible to get to school using the bicycle lanes output -1.

</p><h3>Example</h3>
<pre><b>Input:</b>
3

0 0 5
4 0 3
3.0 4.0
1.878679656440357 -2.121320343559643

0 0 5
4 0 3
4.0 3.0
4.0 -3.0

0 0 4
10 0 4
4.0 0.0
6.0 0.0

<b>Output:</b>
8.4875540166
6.4350110879
-1
</pre>
<img src="/content/turbo:bicycle.png" alt="Illustration of sample test data">