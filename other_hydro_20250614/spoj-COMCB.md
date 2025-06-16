<p>BuggyD has always been fascinated with chess boards (though he really sucks at chess).  He makes an observation that a chess board is complete with respect to knights and rooks and incomplete with respect to bishops (unless the dimensions are 1 ¡Á 1).  A complete chess board is one in which it is possible to traverse all the squares starting from one possible square.  Knights have always been his favourite pieces and he has decided to analyze completeness with respect to knights.  Given the dimesions of the chess board help BuggyD find the lexicographically first path that visits all squares of a chess board with a knight.</p>

<p>Each square must be traversed only once.  Note that a knight can only move two squares in one direction and one square perpendicular to the previous direction.</p>

<h3>Input</h3>
<p>The first line of the input contains an integer <b>t</b>, the number of test cases.  <b>t</b> test cases follow.</p>

<p>Each test case consists of a single line cotaining two integers (<b>X</b> and <b>Y</b>) separated by a single space, specifying the dimensions of the chess board.  The numbers 1 to <b>X</b> denote rows and the capital letters A to Y denote the coloumns. Each square is represented by its column index followed by it's row index - for example, <tt>B4</tt> denotes the square in the 4th row and 2nd column.</p>

<p>The total number of squares on the chess board will be no more than 26.

</p><h3>Output</h3>
<p>For each test case output one line consisting of the lexicographically first path of the knight, or "-1" (quotes for clarity) if the chess board is incomplete with respect to a knight.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
4 5

<b>Output:</b>
A1B3C1A2B4D3E1C2D4E2C3A4B2D1E3C4A3B1D2E4
</pre>