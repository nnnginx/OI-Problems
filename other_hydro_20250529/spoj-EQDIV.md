<p>An equidivision of an n × n square array of cells is a partition of the n^2 cells in the array in exactly n sets, each one with n contiguous cells. Two cells are contiguous when they have a common side.

</p><p><br>A good equidivision is composed of contiguous regions. The figures show a good and a wrong equidivision for a 5×5 square:

</p><p><br></p><center>
<img src="/content/steinersp:equidiv.jpg" alt="subir imagenes" border="0"></center>

<p><br>
Note that in the second example the cells labeled with 4 describe three non-contiguous regions and cells labeled with 5 describe two non-contiguous regions. You must write a program that evaluates if an equidivision of the cells in a square array is good or not.

<br>
</p><h3>Input</h3>
<p>It is understood that a cell in an n×n square array is denoted by a pair (i, j), with 1 &lt;= i, j &lt;= n. The input file contains several test cases. Each test case begins with a line indicating n, 0 &lt; n &lt; 100, the side of the square array to be partitioned. Next, there are n − 1 lines, each
one corresponding to one partition of the cells of the square, with some non-negative integer numbers. 

</p><p><br>Consecutive integers in a line are separated with a single blank character. A line of the form


</p><p><br></p><center>a1 a2 a3 a4 ...</center>

<p><br>
means that cells denoted with the pairs (a1, a2), (a3, a4), ... belong to one of the areas in the partition. The last area in the partition is defined by those cells not mentioned in the n − 1 given lines. If a case begins with n = 0 it means that there are no more cases to analyze.

</p><p><br>
</p><h3>Output</h3>
<p>For each test case good must be printed if the equidivision is good, in other case, wrong must be printed. The answers for the different cases must preserve the order of the input.

<br>
</p><h3>Example</h3>

<pre><b>Input:</b>
2
1 2 2 1
5
1 1 1 2 1 3 3 2 2 2
2 1 4 2 4 1 5 1 3 1
4 5 5 2 5 3 5 5 5 4
2 5 3 4 3 5 4 3 4 4
5
1 1 1 2 1 3 3 2 2 2
2 1 3 1 4 1 5 1 4 2
4 5 5 2 5 3 5 5 5 4
2 4 1 4 3 5 4 3 4 4
0

<b>Output:</b>
wrong
good
wrong
</pre>