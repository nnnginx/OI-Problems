<p align="justify">
</p><p>
     We are given a bar of chocolate composed of <i>m*n</i> square pieces. One should break the chocolate into single squares. Parts of the chocolate may be broken along the vertical and horizontal lines as indicated by the broken lines in the picture. 
</p>
<p>
     A single break of a part of the chocolate along a chosen vertical or horizontal line divides that part into two smaller ones. Each break of a part of the chocolate is charged a cost expressed by a positive integer. This cost does not depend on the size of the part that is being broken but only depends on the line the break goes along. Let us denote the costs of breaking along consecutive vertical lines with <i>x</i><sub>1</sub>, <i>x</i><sub>2</sub>, ...,
<i>x</i><sub><i>m</i>-1</sub> and along horizontal lines with
<i>y</i><sub>1</sub>, <i>y</i><sub>2</sub>, ...,
<i>y</i><sub><i>n</i>-1</sub>. 
</p>
<p>
     The cost of breaking the whole bar into single squares is the sum of the successive breaks. One should compute the minimal cost of breaking the whole chocolate into single squares.
</p>
<img src="/content/thanhvy:chocolate.jpg">

<p>
For example, if we break the chocolate presented in the picture first along the horizontal lines, and next each obtained part along vertical lines then the cost of that breaking will be <i>y</i><sub>1</sub>+<i>y</i><sub>2</sub>+<i>y</i><sub>3</sub>+4*(<i>x</i><sub>1</sub>+<i>x</i><sub>2</sub>+<i>x</i><sub>3</sub>+<i>x</i><sub>4</sub>+<i>x</i><sub>5</sub>).
</p> 

<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="justify">
     <li align="justify">Reads the numbers <i>x</i><sub>1</sub>, <i>x</i><sub>2</sub>, ...,
<i>x</i><sub><i>m</i>-1</sub> and <i>y</i><sub>1</sub>,
<i>y</i><sub>2</sub>, ..., <i>y</i><sub><i>n</i>-1</sub> </li>
     <li align="justify"> Computes the minimal cost of breaking the whole chocolate into single squares, writes the result. </li>
</ul></div>

<h3>Input</h3>
<p>
One integer in the first line, stating the number of test cases, followed by a blank line. There will be not more than 20 tests.
</p>
<p>
For each test case, at the first line there are two positive
integers <i>m</i> and <i>n</i> separated by a single space, 2 &lt;=
<i>m</i>,<i>n</i> &lt;= 1000. In the successive <i>m</i>-1 lines there
are numbers <i>x</i><sub>1</sub>, <i>x</i><sub>2</sub>, ...,
<i>x</i><sub><i>m</i>-1</sub>, one per line, 1 &lt;=
<i>x</i><sub><i>i</i></sub> &lt;= 1000. In the successive <i>n</i>-1 lines there
are numbers <i>y</i><sub>1</sub>, <i>y</i><sub>2</sub>, ...,
<i>y</i><sub><i>n</i>-1</sub>, one per line, 1 &lt;=
<i>y</i><sub>i</sub> &lt;= 1000.
</p>
<p>
The test cases will be separated by a single blank line. 
</p>

<h3>Output</h3>
<p>
For each test case : write one integer - the minimal cost of breaking the whole chocolate into single squares. 
</p>

<h3>Example</h3>

<pre><b>Input:</b>
1

6 4
2
1
3
1
4
4
1
2

<b>Output:</b>
42
</pre>