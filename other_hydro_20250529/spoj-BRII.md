<p>Problem <a href="/problems/BRI/">BRIDGE</a> has shown that you are able to build the cheap bridge through the river very quickly. Now you will not have problems with time limit. You will have problems with number of bridges.</p>

<p style="text-align: center;"><img src="../../content/shkoorah:bridge2.png" alt=""></p>

<h3>Input</h3>
<p>There is a single positive integer <i>T</i> on the first line of input. It stands for the number of test cases to follow. Each test case is exactly five lines, containing description of the route between two cities A and B, located on opposite sides of the rivers.</p>

<p><i>
n<br>
a<sub>0</sub> a<sub>1</sub> a<sub>2</sub> ...  a<sub>n</sub><br>
h<sub>1</sub> h<sub>2</sub> ...  h<sub>n</sub><br>
c<br>
s<sub>0</sub> s<sub>1</sub> s<sub>2</sub> ...  s<sub>n</sub><br>
</i></p>

<p>Here <i>n</i> is the number of the rivers which are parallel to each other, <i>a<sub>i</sub></i> - the distances between rivers or between rivers and cities, <i>h<sub>i</sub></i> - the widths of the rivers, <i>c</i> - the distance between A and B along the axis parallel to the river, <i>s<sub>i</sub></i> - the costs of the unit of the bridge through <i>i<sub>th</sub></i> river and <i>s<sub>0</sub></i> - the cost of the unit of the road. Example for <i>n</i>=2 you can see on the picture.</p>

<p>All integers in input are positive and less than 50, except <i>c</i> - it is less than 2000.</p>


<h3>Output</h3>
<p>For each test case your program should write a single number to the standard output, equal to the minimal total cost of the route between A and B, accurate up to two digits after the decimal dot.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
2
1 1 1
1 1
1
1 1 1

<b>Output:</b>
5.10
</pre>