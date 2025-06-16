<p>Eefun is an accountant. As an accountant, he loves to work with spreadsheet. In spreadsheet, a data must be saved into a single cell which has row and column. Spreadsheet has an interesting feature. It can move the cursor from a cell to another cell by clicking a button based on this rules :</p>
<p>- <b>If current cell has a data and it's right neighbour also contain data,</b> then clicking the right button will make the cursor to move to the first cell in the right of current cell which it's right neighbour doesnt contain a data. If there is no such cell, then the cursor will move to the rightmost cell in the current row.</p>
<p>- <b>Else,</b> then clicking the right button will make the cursor to move to the first cell in the right of current cell which has a data. If there is no such cell, then the cursor will move to the rightmost cell in the current row.</p>
<p>Same rules apply when clicking the left, up, and down button.</p>
<p>Eefun realizes this feature which makes him curious. He currently has a lot of data in his spreadsheet. He wants to edit a data on cell (R,C), but first he must move his cursor to the desired cell. Currently his cursor is at cell (1,1), the top-leftmost cell in the spreadsheet. Eefun wants to know the minimal number of button clicked to reach the cell.</p>
<h3>Input</h3>
<p>First line of input consists of 2 integers, N and M, the number of rows and number of columns<br>Second line consists of a number X, the number of data that Eefun currently has.<br>Next N lines each consists of 2 integers, A and B which denotes the position of the data<br>Line (N+3) contains a number Q, the number of query.<br>Next Q lines each consists of 2 integers, R and C, the position of cells that Eefun wants to edit&nbsp;</p>
<h3>Output</h3>
<p>For each query, output a single integer, the minimum number of buttons that Eefun should click to reach cell (R,C). If the cell cannot be reached, then output a string "Eefun gagal mengedit data"<br>"Eefun gagal mengedit data" means "Eefun fails to edit his data"&nbsp; <br>
<b>Note that each query is independent, so Eefun's initial cursor will be at (1,1) for each query</b></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 3
8
1 1
1 2
1 3
2 1
2 3
3 1
3 2
3 3
2
3 2
1 3

<strong>Output:</strong>
Eefun gagal mengedit data<br>1&nbsp;</pre>

<b>Note : You can try this in Microsoft Excel using ctrl + arrow button</b>
<div style="border: 1px solid #FC0; background-color: #FFC; padding: 5px; margin-bottom: 10px;">
<h3>Constraints:</h3>
<ul>
<li>1 ¡Ü X ¡Ü min(100.000 , N*M)</li>
<li>1 ¡Ü N,M ¡Ü 10.000</li>
<li>1 ¡Ü Q ¡Ü 100.000</li>
</ul>
</div>