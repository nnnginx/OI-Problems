<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/GANNHAT/en/">English</a></td> 
<td width="50%"><a href="/problems/GANNHAT/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p>The manhattan distance between two points A(x<sub>1</sub>,y<sub>1</sub>) and B(x<sub>2</sub>,y<sub>2</sub>) is defined as following:</p>
<p style="text-align:center;">D(A,B) = |x<sub>1</sub> - x<sub>2</sub>| + |y<sub>1</sub> - y<sub>2</sub>|</p>
<p>Given N points A<sub>1</sub>, A<sub>2</sub>, ..., A<sub>N</sub>, 
for each point A<sub>i</sub> you need to calculate the minimum D(A<sub>i</sub> , A<sub>j</sub>) (j ¡Ù i).</p>

<h3>Input</h3>
<ul>
<li>The first line contains a positive integer N (1 ¡Ü N ¡Ü 200000).
</li><li>The i-th line of the next N lines contains two integers x and y which are co-ordinates of the i-th point(0 ¡Ü x, y ¡Ü 10<sup>7</sup>)
</li></ul> 

<h3>Output</h3>
<ul>
<li>Print N lines, in which the i-th line contains the minimum distance for the i-th point. 
</li></ul> 

<h3>Example</h3>

<pre><b>Input:</b>
4
0 0
0 1
1 0
1 1

<b>Output:</b>
1
1
1
1
</pre>