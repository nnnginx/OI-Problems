<p style="text-align: left;">Two rooks are to be placed on a chess like N*N game board . each square contains a single non negative integer . the rooks must be placed on different squares.</p>
<p style="text-align: left;">We say that some squares on the board are attacked if that square in the same row or same column with the rook but squares containing rooks are not attacked.</p>
<p style="text-align: left;">We want to place our rooks so that the total sum of the numbers of all attacked squares is as large as possible . write a program that will find this maximum sum.</p>
<p align="right">&nbsp;</p>
<h3>Input</h3>
<p style="text-align: left;">The first line on input will contain N , 2&lt;=N&lt;=300</p>
<p style="text-align: left;">Each of the following N lines N integers . each number will be greater than or equal zero and less that 1000 these are numbers on board</p>
<p align="right">&nbsp;</p>
<h3>Output</h3>
<p style="text-align: left;">the only line should contain single integer ¨C the maximum sum from the task description</p>
<p align="right">&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3</pre>
<pre>0 1 4</pre>
<pre>3 0 2</pre>
<pre>1 4 1

<strong>Output:</strong>
15
</pre>