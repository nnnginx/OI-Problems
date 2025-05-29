<p>A sudoku goblin has read your book with sudoku problems. He has erased or added some numbers from settings. Your task is to write a program that can detect modified settings.</p>
<p>For every sudoku setting you have to count number of possible solutions and in the case that it is equal to 1 print</p>
<p>the unique solution.</p>
<h3>Input</h3>
<p>There is a number T of the test cases on the first line folowed by T sudoku tables separated by one empty line. One sudoku table consists of 9 lines of 9 numbers 0-9 separated by one space. Zero in the table marks the empty field.</p>
<h3>Output</h3>
<p>For every test case, one line with number of possible solutions optionally followed by solved sudoku in the same format as on the input.</p>
<h3>Example</h3>
<p>&nbsp;</p>
<pre><strong>Input:</strong><br>3<br>3 0 6 0 0 2 5 0 0<br>0 0 0 0 3 8 0 0 0<br>7 0 8 0 1 6 0 9 0<br>0 0 7 0 0 3 8 6 0<br>8 2 0 0 7 0 0 4 5<br>0 6 3 1 0 0 9 0 0<br>0 7 0 3 5 0 6 0 2<br>0 0 0 8 2 0 0 0 0<br>0 0 2 9 0 0 7 0 4<br><br>3 0 6 0 0 2 5 0 3<br>0 0 0 0 3 8 0 0 0<br>7 0 8 0 1 6 0 9 0<br>0 0 7 0 0 3 8 6 0<br>8 2 0 0 7 0 0 4 5<br>0 6 3 1 0 0 9 0 0<br>0 7 0 3 5 0 6 0 2<br>0 0 0 8 2 0 0 0 0<br>0 0 2 9 0 0 7 0 4<br><br>3 0 6 0 0 2 0 0 0<br>0 0 0 0 3 8 0 0 0<br>7 0 8 0 1 6 0 9 0<br>0 0 7 0 0 3 8 6 0<br>8 2 0 0 7 0 0 4 5<br>0 6 3 1 0 0 9 0 0<br>0 7 0 3 5 0 6 0 2<br>0 0 0 8 2 0 0 0 0<br>0 0 2 9 0 0 7 0 4<br><br>&nbsp;<strong>Output:</strong>
1<br>3 1 6 4 9 2 5 7 8 <br>2 9 5 7 3 8 4 1 6 <br>7 4 8 5 1 6 2 9 3 <br>9 5 7 2 4 3 8 6 1 <br>8 2 1 6 7 9 3 4 5 <br>4 6 3 1 8 5 9 2 7 <br>1 7 9 3 5 4 6 8 2 <br>6 3 4 8 2 7 1 5 9 <br>5 8 2 9 6 1 7 3 4 <br>0<br>2</pre>