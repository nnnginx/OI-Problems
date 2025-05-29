<p>A N¡ÁN matrix is filled with numbers 1 to N<sup>2</sup>, diagonally in a zig-zag fashion.</p>
<p>The table below shows numbers in the matrix for N = 6.</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="34">
<p style="text-align: center;">1</p>
</td>
<td width="34">
<p style="text-align: center;">2</p>
</td>
<td width="34">
<p style="text-align: center;">6</p>
</td>
<td width="34">
<p style="text-align: center;">7</p>
</td>
<td width="34">
<p style="text-align: center;">15</p>
</td>
<td width="34">
<p style="text-align: center;">16</p>
</td>
</tr>
<tr>
<td width="34">
<p style="text-align: center;">3</p>
</td>
<td width="34">
<p style="text-align: center;">5</p>
</td>
<td width="34">
<p style="text-align: center;">8</p>
</td>
<td width="34">
<p style="text-align: center;">14</p>
</td>
<td width="34">
<p style="text-align: center;">17</p>
</td>
<td width="34">
<p style="text-align: center;">26</p>
</td>
</tr>
<tr>
<td width="34">
<p style="text-align: center;">4</p>
</td>
<td width="34">
<p style="text-align: center;">9</p>
</td>
<td width="34">
<p style="text-align: center;">13</p>
</td>
<td width="34">
<p style="text-align: center;">18</p>
</td>
<td width="34">
<p style="text-align: center;">25</p>
</td>
<td width="34">
<p style="text-align: center;">27</p>
</td>
</tr>
<tr>
<td width="34">
<p style="text-align: center;">10</p>
</td>
<td width="34">
<p style="text-align: center;">12</p>
</td>
<td width="34">
<p style="text-align: center;">19</p>
</td>
<td width="34">
<p style="text-align: center;">24</p>
</td>
<td width="34">
<p style="text-align: center;">28</p>
</td>
<td width="34">
<p style="text-align: center;">33</p>
</td>
</tr>
<tr>
<td width="34">
<p style="text-align: center;">11</p>
</td>
<td width="34">
<p style="text-align: center;">20</p>
</td>
<td width="34">
<p style="text-align: center;">23</p>
</td>
<td width="34">
<p style="text-align: center;">29</p>
</td>
<td width="34">
<p style="text-align: center;">32</p>
</td>
<td width="34">
<p style="text-align: center;">34</p>
</td>
</tr>
<tr>
<td width="34">
<p style="text-align: center;">21</p>
</td>
<td width="34">
<p style="text-align: center;">22</p>
</td>
<td width="34">
<p style="text-align: center;">30</p>
</td>
<td width="34">
<p style="text-align: center;">31</p>
</td>
<td width="34">
<p style="text-align: center;">35</p>
</td>
<td width="34">
<p style="text-align: center;">36</p>
</td>
</tr>
</tbody>
</table>
<p>There is a rabbit in the cell containing number 1. A rabbit can jump to a neighboring cell (up, down, left or right) if that cell exists.</p>
<p>Given K valid rabbit jumps, write a program that will calculate the sum of numbers of all cells that rabbit visited (add the number to the sum each time rabbit visits the same cell).&nbsp;</p>
<h3>Input</h3>
<p>The first line contains two integers N and K (1 ¡Ü N ¡Ü 100<span style="font-size: 4.0pt; line-height: 110%;"> </span>000, 1 ¡Ü K ¡Ü 300<span style="font-size: 4.0pt; line-height: 110%;"> </span>000), the size of the matrix and the number of rabbit jumps.</p>
<p>The second line contains a sequence of K characters 'U', 'D', 'L' and 'R', describing the direction of each jump. The sequence of jumps will not leave the matrix at any moment.</p>
<h3>Output</h3>
<p>Output one integer, the sum of numbers on visited cells.</p>
<p><strong>Note:</strong> This number doesn't always fit in 32-bit integer type.</p>
<h3>Example</h3>
<table style="width: 100%;" border="0" frame="void" align="center">
<tbody>
<tr>
<td align="left" valign="top">
<pre><strong>Input:</strong>
6 8
DDRRUULL

<strong>Output:</strong>
47</pre>
</td>
<td align="left" valign="top">
<pre><strong>Input:</strong>
3 8
DDRRUULL

<strong>Output:</strong>
41</pre>
</td>
<td align="left" valign="top">
<pre><strong>Input:</strong>
6 10
RRRRRDDDDD

<strong>Output:</strong>
203</pre>
</td>
</tr>
</tbody>
</table>
<p><strong>Clarification for the first sample:</strong> The rabbit visits cells 1, 3, 4, 9, 13, 8, 6, 2 and 1. <strong>Clarification for the second sample: </strong>The rabbit visits cells 1, 3, 4, 8, 9, 7, 6, 2 and 1. <strong>Clarification for the third sample: </strong>The rabbit visits cells 1, 2, 6, 7, 15, 16, 26, 27, 33, 34 and 36.</p>