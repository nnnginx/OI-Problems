<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MTEMP/en/">English</a></td>
<td width="50%"><a href="/problems/MTEMP/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p>
</p><pre>There is a rectangular area containing n ¡Á m cells. Two cells are marked
with ¡°2¡±, and another two with ¡°3¡±. Some cells are occupied by obstacles. 
You should connect the two ¡°2¡±s and also the two ¡°3¡±s with non-intersecting
lines. Lines can run only vertically or horizontally connecting centers
of cells without obstacles.

Lines cannot run on a cell with an obstacle. Only one line can run on
a cell at most once. Hence, a line cannot intersect with the other line, 
nor with itself. Under these constraints, the total length of the two
lines should be minimized. The length of a line is defined as the
number of cell borders it passes. In particular, a line connecting cells
sharing their border has length 1.

Fig. 1(a) shows an example setting. Fig. 1(b) shows two lines satisfying the
constraints above with minimum total length 18.

<img src="../../../../../../content/simes:MMAHWIRE.png" border="0">

Figure 1: An example of setting and its solution
</pre>
<h3>Input</h3>
<pre>The input consists of multiple datasets, each in the following format.

    n	m
    row1
    ¡­
    rown

n is the number of rows which satisfies 2 ¡Ü n ¡Ü 9. m is the number of columns
which satisfies 2 ¡Ü m ¡Ü 9. Each rowi is a sequence of m digits separated by
a space. The digits mean the following.

    0: Empty

    1: Occupied by an obstacle

    2: Marked with ¡°2¡±

    3: Marked with ¡°3¡±

The end of the input is indicated with a line containing two zeros separated
by a space.

SAMPLE INPUT
5 5
0 0 0 0 0
0 0 0 3 0
2 0 2 0 0
1 0 1 1 1
0 0 0 0 3
2 3
2 2 0
0 3 3
6 5
2 0 0 0 0
0 3 0 0 0
0 0 0 0 0
1 1 1 0 0
0 0 0 0 0
0 0 2 3 0
0 0
</pre>
<h3>Output</h3>
<pre>For each dataset, one line containing the minimum total length of the two
lines should be output. If there is no pair of lines satisfying the requirement,
answer ¡°0¡± instead.  

Sample Output

18
2
17
</pre>