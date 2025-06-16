<p>
One has to cut out a number of rectangles from a paper square. The sides of each rectangle are to be parallel 
to the sides of the square. Some rectangles can be already cut out. What is the largest area of a rectangle 
which can be cut out from the remaining paper? 
</p>
<h3>Illustration</h3>
<p>
Three rectangles have been cut out from the square 10x10 in the figure shown below. The area of the largest 
rectangle that can be cut out from the remaining paper is 16. One of such rectangles is shown with a dashed 
line. 
</p>
<img src="/content/adrian:CUTOUT.png" align="left/"> 
<h3>Task</h3>
<p>
Write a program that for each data set from a sequence of several data sets:
</p>
<div align="justify">
<ul>
<li>reads descriptions of a square and rectangles from the input, 
</li><li>computes the area of the largest rectangle which can be cut out from the remaining paper, 
</li><li>writes the result to output.</li> 
</ul>
</div>
<h3>Input</h3>
<p>
The first line of the input file contains one positive 
integer d not larger than 10. This is the number of data sets. The data sets 
follow. Each set of data occupies two consecutive lines of the input file. The 
first line of each data set contains two integers n and r, 1 &lt;=
                     
                    
           n &lt;=   40000, 0 &lt;= r &lt;= 100. The integer n is the length 
of the sides of an input square. The integer r is the number of rectangles which have been cut out from the 
square. The second line of the data set contains a sequence of 4r integers x<sub>1</sub>, x<sub>2</sub>,...,x<sub>4r</sub> from the interval 
[0,n] separated by single spaces. For each i = 1,...,r, integers x<sub>4i-3</sub>, x<sub>4i-2</sub>, x<sub>4i-1</sub>, x<sub>4i</sub>
describe the i-th rectangle: x<sub>4i-3</sub> is the distance of its left side from the left side of the square, x<sub>4i-2</sub>
is the distance of its right side from the left side of the square, x<sub>4i-1</sub> is the distance of the bottom side of the rectangle from the 
bottom side of the square and x<sub>4i</sub> is the distance of its top side from the bottom side of the square. 
</p>
<h3>Output</h3>
<p>
For each i = 1,...,d, your program should write only one integer to the i-th line of the output file -- the 
largest area of a rectangle which can be cut out from the rest of the i-th square. 
</p>
<h3>Example</h3>
<pre>Sample input:

2 
6 2 
0 3 0 3 3 6 3 6 
10 3 
0 5 0 5 0 10 5 10 9 10 0 5 

Sample output:

9 
20 
</pre>