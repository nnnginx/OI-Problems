<p align="left">
The city of <b>Y-O</b> is a network of two-way streets and junctions with the following properties:

</p><ol>
<li> There is no more than one street between each pair of junctions.
</li><li> Every junction is connected to every other junction either directly via a street or through other junctions by a unique path.
</li><li> When a light is placed at a junction, all the streets meeting at this junction are also lit.
</li></ol>
<p></p>

<p align="left">
A valid lighting is a set of  junctions such that if lights were placed at these, all the streets would be lit.
An optimal lighting is a valid lighting such that it contains the least number of junctions.
</p>

<p align="left">
The task is divided into two subtasks:
</p><ol>
<li> Find the number of lights in an optimal lighting.
</li><li> Find the total number of such optimal lightings in the city.
</li></ol>
<p></p>

<h3>Input</h3>

<ul>
<li> The first line of the input contains a positive integer <b>t &lt;= 20</b>, denoting the number of test cases.
</li><li> The description of the test cases follows one after the other.


</li><li><b>Network Description:</b>
<ul> 
<li> The first line of description of a network consists of a positive integer <b>n &lt;= 100010</b> denoting the number of junctions in the network. 
</li><li> Each junction is numbered with a unique integer between <b>1</b> and <b>n</b>.
</li><li> The following <b>n-1</b> lines contain a pair of integers <b>u v (1 &lt;= u,v  &lt;=  n)</b> separated by a single space denoting that there is a street between junction <b>u</b> and junction <b>v</b>.
</li></ul>
</li></ul>
<p></p>

<h3>Output</h3>
<p align="left">
The output must consist of <b>t</b> lines, the <b>k<sup>th</sup></b> line corresponding to the <b>k<sup>th</sup></b> network; <b>(1 &lt;= k &lt;= t)</b>.
The <b>k<sup>th</sup></b> line must contain two integers separated by a single space.
The first integer on the <b>k<sup>th</sup></b> line must be the number of junctions in an optimal lighting of network <b>k</b>.
The second integer must be <b>N%10007</b>, which is the remainder left by the number of optimal lightings when divided by <b>10007</b>.
</p>

<h3>Example</h3>

<tt>
<p align="left">
<b>Input:</b>

<br>2
<br>4
<br>1 2
<br>2 3
<br>3 4
<br>3
<br>1 2
<br>1 3

</p>

<p align="left">

<b>Output:</b>
<br>2 3
<br>1 1
</p>
</tt>