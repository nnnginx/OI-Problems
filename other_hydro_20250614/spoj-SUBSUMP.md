<p>You are given a <strong>N x N</strong> grid, where each cell in the grid is either blocked or free. You can place any number between <strong>1</strong> to <strong>N</strong> in the free cells. You are required to assign numbers to the free cells. No free cells should be left empty after the assignment, i.e. each free cell must contain exactly one number from the range <strong>[1-N]. </strong>
<br><br>

You are also given a target value <strong>V</strong>. Find out how many ways we can assign numbers to the free cells such that their sum equals <strong>V</strong>. It is also required to satisfy the following constraints:
<br><br>
</p><ol>
  <li>For any row, all the numbers present in that row should be distinct.</li>
  <li>For any column, all the numbers present in that column should be distinct.</li>
</ol> 
<br><br>
Two ways are considered different if <strong>any</strong> particular cell has different values assigned.
<br><br>
Let  <strong>M</strong> denote the total number of free cells. It is guaranteed that there will be at least  <strong>1</strong> and no more than  <strong>12 </strong> free cells.

<h3>Input</h3>
The first line contains an integer <strong>T</strong>, denoting the number of test cases. The next line contains two integers, <strong>N</strong> and <strong>V</strong>. The next <strong>N</strong> lines contains the grid, each line contains the corresponding row of the grid.
<br><br>
Cells marked with a <strong>'.'</strong> indicates free cells, and cells marked as <strong>'X'</strong> denotes blocked cells. Each cell can be either blocked or free so the grid will not contain any other extra characters.

<h3>Constraints</h3>
<strong><li>1 &lt; T ¡Ü 120</li></strong>
<strong><li>1 &lt; N ¡Ü 12</li></strong>
<strong><li>1 &lt; V ¡Ü 144</li></strong>
<strong><li>1 &lt; M ¡Ü 12</li></strong>

<br><br>
For <strong>60%</strong> of the test cases, the following constraints will hold:
<strong><li>1 &lt; N ¡Ü 8</li></strong>
<strong><li>1 &lt; M ¡Ü 8</li></strong>

<h3>Output</h3>
For each test case, output the case number followed by the number of ways to create the assignment. Please check the sample input/output for more clarity.

<h3>Example</h3>
<pre><b>Input:</b>
5
1 1
.
2 2
.X
.X
2 3
.X
X.
3 7
.X.
X.X
XX.
5 15
XX.XX
XX.XX
.XXX.
XX.XX
XX.XX

<b>Output:</b>
Case 1: 1
Case 2: 0
Case 3: 2
Case 4: 9
Case 5: 192
</pre>