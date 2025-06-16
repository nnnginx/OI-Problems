<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/PA06ANT/en/">English</a></td>
<td width="50%"><a href="/problems/PA06ANT/vn/">Tiếng Việt</a></td> 
</tr></tbody></table>


<p>
A Byteotian ant is walking along the edges of ABCDEFGH cube: <br>
</p><center>
<img src="./23746/file/XYAEJsJt.png">
</center>
<p></p>

<p>It tries to find out, in how many ways it can go from one given vertex, to another given vertex, walking along exactly <b>k</b> edges (when the ant enters an edge, it will not turn back and will finally reach the second end of this edge). If the ant goes through some edge <b>x</b> times, we count this edge <b>x</b> times. The ant would like to have interesting routes, that is if the ant is in some vertex, it would like to leave this vertex using an edge other than the edge recently used to enter this vertex (i.e. it want not to use the same edge twice in a row).
</p>

<p>
Our ant is not so smart, because it can only count using integers from <b>0</b> to <b>p-1</b>, for some <b>p</b>, so you should compute the result modulo <b>p</b>.
</p>

<h3>Request</h3>
<p>
Write a program which:<br>
    * reads the starting and the ending vertex of the ant's route, number of edges on the ant's route, and integer <b>p</b>,<br>
    * computes number of interesting routes, which satisfy the ant's requests, modulo <b>p</b>,<br>
    * writes the answer to the standard output.
</p>

<h3>Input</h3>
<p>
The first line of the standard input contains two capital English letters <b>v<sub>1</sub></b> and <b>v<sub>2</sub></b>, separated by a single space. The two letters denote the starting and ending vertex of the ant's route respectively. The second line contains two integers <b>k</b> and <b>p</b>, separated by a single space.
</p>

<h3>Output</h3>
<p>
Exactly one integer is to be written on the standard output. This integer is the number of interesting routes from the vertex <b>v<sub>1</sub></b> to the vertex <b>v<sub>2</sub></b>, containing exactly <b>k</b> edges, modulo <b>p</b>.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
A B
3 100

<b>Output:</b>
2
</pre>

<p>
</p><center>
<img src="./23746/file/7kIQVelh.png">
</center>
<p></p>

<h3>Limitations</h3>
<p>
* A ≤ v<sub>1</sub>, v<sub>2</sub> ≤ H, v<sub>1</sub> ≠ v<sub>2</sub>.<br>
* 1 ≤ k ≤ 2 x 10<sup>9</sup>, 2 ≤ p ≤ 10<sup>9</sup>.<br>
</p>