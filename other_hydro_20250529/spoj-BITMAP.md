<p>
There is given a rectangular bitmap of size <i>n*m</i>. Each pixel of the bitmap is either white or black, but at least one is white. The pixel in
<i>i</i>-th line and <i>j</i>-th column is called the pixel (<i>i,j</i>). The distance between two pixels
<b>   p<sub>1</sub></b>=(<i>i<sub>1</sub>,j<sub>1</sub></i>) and <b>p<sub>2</sub></b>=(<i>i<sub>2</sub>,j<sub>2</sub></i>) is defined as:
</p>

<p></p><center>
d(<b>p<sub>1</sub></b>,<b>p<sub>2</sub></b>)=|<i>i<sub>1</sub>-i<sub>2</sub></i>|+|<i>j<sub>1</sub>-j<sub>2</sub></i>|.
</center><p></p>

<h3>Task</h3> 

<p>
Write a program which:
</p><ul>  
 <li>reads the description of the bitmap from the standard input,
 </li><li>for each pixel, computes the distance to the nearest white pixel,
 </li><li>writes the results to the standard output. 
</li></ul>  

<h3>Input</h3> 

<p>
The number of test cases t is in the first line of input, then t test cases follow separated by an empty line.

In the first line of each test case there is a pair of integer numbers<i>
n, m</i> separated by a single space, <i> 1&lt;=n &lt;=182</i>, <i> 1&lt;=m&lt;=182</i>. In each of the following
<i> n</i> lines of the test case exactly one zero-one word of length
<i> m,</i> the description of one line of the bitmap, is written. On the <i>j</i>-th position in the line
(<i>i+1</i>), <i> 1 &lt;= i &lt;= n</i>, <i> 1 &lt;= j &lt;= m</i>, is '1' if, and only if the pixel
(<i>i,j</i>) is
white.
</p>

<h3>Output</h3>

<p>
In the <i>i</i>-th line for each test case, <i> 1&lt;=i&lt;=n</i>, there
should be written
<i> m</i> integers f(<i>i,1</i>),...,f(<i>i,m</i>) separated by single spaces, where f(<i>i,j</i>) is
the distance from the pixel
(<i>i,j</i>) to the nearest white
pixel.
</p>

<h3>Example</h3>

<pre><b>Sample input:</b>
1
3 4
0001
0011
0110

<b>Sample output:</b>
3 2 1 0
2 1 0 0
1 0 0 1
</pre>