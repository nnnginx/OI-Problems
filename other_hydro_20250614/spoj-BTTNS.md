<p><br>Luis has a new toy, is a weird board with NxM cells. The cells can be white or<br>black.<br>Each cell has a button inside, when you press a button every cell with Manhattan<br>distance equal or less than K to the cell with the button pressed change of color<br>( white to black, or black to white ).<br>At the beginning, every cell is white but somebody pressed some buttons and now<br>the board has some black cells.<br>Help Luis to find how many buttons were pressed.<br>You can assume that no button will be pressed two or more times.<br>There will be always only one configuration of buttons pressed that generate the<br>final board.</p>
<h3>Input</h3>
<p>The first line of input contains an integer t&lt;=10, the number of test cases. It is<br>followed by t test cases, each consisting of N+1 lines. The first line of each case<br>contains three integers N,M,K separated by space (1&lt;=N,M&lt;=20 , 0&lt;=K&lt;=20).<br>The next N lines contains M integers, each integer can be 0 or 1, the final state of<br>each cell. ( 0 is white, 1 is black )</p>
<h3>Output</h3>
<p>For each case, output a single line consisting of the number of buttons pressed.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>2 2 0<br>1 0<br>0 1<br>2 2 1<br>1 1<br>1 1

<strong>Output:</strong>
2<br>4
</pre>