<p>Even though he has found all the most amusing rides, Mirko‟s enthusiasm still isn‟t fading. He opened his graph paper notebook and started colouring squares, and a new, even harder problem dawned on him.</p>
<p>You are given a square table consisting of N rows by N columns. Each cell is either black or white. A set of cells forming a rectangle, with horizontal and vertical edges following cell borders, shall be called a black rectangle if all cells inside the rectangle are black and it consists of at least two cells.</p>
<p><img src="../../../../../../content/simes:C2CRNI_left.png"><img src="../../../../../../content/simes:C2CRNI_right.png"></p>
<p>The left image shows two rectangles which are not black rectangles. The rectangle labelled 1 is not a black rectangle because it contains a white cell, and the rectangle labelled 2 is not a black rectangle because it consists of only one cell. On the other hand, the right image shows three valid black rectangles.</p>
<p>Calculate the number of possible selections of two black rectangles that have no common cells. As the required number can be extremely large, you should output the remainder of dividing that number by 10 007.</p>
<h3>Input</h3>
<p>The first line of input contains the integer N (2 ≤ N ≤ 1000).</p>
<p>Each of the next N lines contains a single row of the table, consisting of N symbols. The symbol 'C' represents a black cell, while 'B' represents a white cell.</p>
<h3>Output</h3>
<p>The first and only line of output must contain the remainder of dividing the required number by 10 007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2 <br>CC <br>CC<br><br><strong>Output:</strong><br>2<br><strong><br>Input:</strong><br>3 <br>CCB <br>CCB <br>CBB<br><br><strong>Output:</strong><strong><br></strong>5<br><strong><br>Input:</strong><strong><br></strong>5<br>BCCBB<br>BBCBB<br>BCCBB<br>BBBBB<br>CCBBB<br><br><strong>Output:</strong><br>8</pre>