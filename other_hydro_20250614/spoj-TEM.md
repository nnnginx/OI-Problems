<p> After many years of hard work a group of scientists developed a shiny new state-of-the-art processor with a 3D configuration. Due to the high clock frequency at which this processor works, the silicon cube uses up too much energy. Even with its powerful cooling system, the processor is unable to cope with the heat discharge in some of its cubical blocks. With the help of special analysis methods, scientists have developed the overheat rate for each of the cubical blocks of the system. As it conveniently happens, this overheat rate is an integer value, either positive or negative depending on many factors (such as the proximity of ventilators, refrigerators, etc.).</p><p>
Science can do no more, so now the developers of the processor need your support. For a given three-dimensional matrix representing the overheat rate of elements of the processor, you have to find a submatrix for which the sum of overheat rates coming from all its elements is maximal.</p>

<h3>Input</h3>
<p><i>t</i> ¨C number of test cases [<i>t</i> &lt;= 99], then t tests follow. <br>
Each test begins with 3 integers: x, y, z ¨C the width, length and height of matrix [5 &lt;= x, y, z &lt;= 50]. Then there follows the description of x rectangular 2D matrixes of height y and width z. In total there are x*y*z integers, which absolute value does not exceed 10000.
</p>

<h3>Output</h3>
<p>For each test case you should output 6 integers: x1, y1, z1, x2, y2, z2, where each triple (xi, yi, zi) defines one of the two opposite corners of submatrix, resulting in the maximum overheat. [1 &lt;= x1 &lt;= x2 &lt;= x] [1 &lt;= y1 &lt;= y2 &lt;= y] [1 &lt;= z1 &lt;= z2 &lt;= z]

</p><h3>Example</h3>

<pre><b>Input:</b>
1
5 5 5
1 1 1 1 1
1 1 1 1 1
1 1 1 1 1
1 1 1 1 1
1 1 1 1 1
-1 -1 -10 -1 -1
-1 -1 -10 -1 -1
-1 -1 -10 -1 -1
-1 -1 -10 -1 -1
-1 -1 -10 -1 -1
20 2 2 2 20
20 2 2 2 20
20 2 2 2 20
20 2 2 2 20
20 2 2 2 20
5 5 5 5 5
5 5 5 5 5
1 1 1 1 1
1 1 1 1 1
1 1 1 1 1
-10 10 -10 10 -10
-10 10 -10 10 -10
-10 10 -10 10 -10
-10 10 -10 10 -10
-10 10 -10 10 -10


<b>Output:</b>
3 1 1 4 5 5 

<b>Note:</b>
The maximum overheat for the example is equal to 295.
</pre>