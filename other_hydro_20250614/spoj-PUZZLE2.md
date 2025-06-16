<p>Sam loves all kinds of puzzles. Recently he received a very special puzzle - a grid of N x M squares, each square is occupied either by a red or by a blue pebble. The puzzle is controlled by several buttons. </p>

<p>Each row of the grid has its corresponding black button. When you press a black button, a complicated mechanism of the puzzle flips the colors of all pebbles in the row corresponding to that button (all red pebbles in this row become blue and vice versa). </p>

<p>Each column of the grid has its corresponding white button. When you press exactly two white buttons simultaneously, the puzzle mechanism exchanges the contents of the two columns corresponding to those buttons without changing the order of the pebbles in the columns. </p>

<p>Sam has found the puzzle very interesting. Unfortunately, he lent it to his daughter Ann yesterday. She was able to understand the idea of the puzzle very quickly and she gave him this teasing task. She drew two arrangements - initial and final and she changed the colors of the pebbles according to the initial arrangement. Sam's task is to decide whether there exists a sequence of puzzle operations which transforms the initial arrangement of the puzzle to the final arrangement. </p>

<h3>Input file specification</h3>
<p>The input file contains several blocks of input data. The first line of the input file contains K - the number of blocks. The first line of each block contains integers N(1&lt;=N&lt;=100) and M(1&lt;=M&lt;=100). Each of the next N lines contain M words (either RED or BLUE), describing the initial Ann's arrangement of the colors of the pebbles. One blank line follows. The next N lines contain M words corresponding to the final arrangement of the colors. </p>

<h3>Output file specification</h3>
<p>The output file contains K lines, the i-th line corresponds to the i-th block of the input data. Each line contains either YES or NO, the answer to the Ann's question. </p>

<h3>Example</h3>
<pre><b>Input file:</b>
2
3 4
BLUE RED BLUE RED
RED BLUE BLUE RED
BLUE BLUE BLUE BLUE

BLUE RED BLUE RED
RED RED BLUE BLUE
BLUE BLUE BLUE BLUE
2 2
BLUE BLUE
BLUE RED

RED RED
RED RED

<b>Output file </b>
YES
NO

</pre>
<p>Note: In the first block of the input data it suffices to use the black button for the second row and then to press the white buttons for the first and the third columns simultaneously. </p>