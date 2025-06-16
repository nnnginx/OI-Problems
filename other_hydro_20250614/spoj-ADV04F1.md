<p>There is a n ¡Á 1 board. Its cells are numbered with integers from 1 to n. First four cells have indistinguishable chips in them. In one turn you can move one chip to the neighbouring cell or move it symmetrically relatively any other chip (i.e. if you move a chip in cell 10 symmetrically relative to the chip in cell 13 it will end up in cell 16), given that the chip won't leave the board and each cell will have no more than one chip. You need to determine the minimum number of turns needed to reach a certain configuration of chips.

</p><h3>Input</h3>
<p>The first line of input contains number T - the amount of test cases. Next T lines consist of four integers a<sub>1</sub>, a<sub>2</sub>, a<sub>3</sub> and a<sub>4</sub> ¡ª the numbers of cells where the chips should be in the final configuration.

</p><h3>Constraints</h3>
<p>1 &lt;= T &lt;= 10000<br>
1 &lt;= a<sub>1</sub> &lt; a<sub>2</sub> &lt; a<sub>3</sub> &lt; a<sub>4</sub> &lt;= n<br>
n = 70

</p><h3>Output</h3>
<p>For each test case print single integer - the answer to the problem in the statement.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
1 2 3 4
1 3 4 6

<b>Output:</b>
0
1

</pre>