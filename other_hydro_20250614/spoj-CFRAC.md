<p>A simple continuous fraction has the form:
<br><br>
</p><center><img src="/content/steinersp:cfrac.jpg" alt="subir imagenes" border="0"></center>

<p><br><br>where the ai’s are integer numbers.

</p><p><br>The previous continuous fraction could be noted as [a1, a2, . . . , an]. It is not difficult to show that any rational number p / q , with integers p &gt; q &gt; 0, can be represented in a unique way by a simple continuous fraction with n terms, such that p / q = [a1, a2, . . . , an−1, 1], where n and the ai’s are positive natural numbers.

</p><p><br>Your task is to find and print the simple continuous fraction that corresponds to a given rational number.

<br>
</p><h3>Input</h3>
<p>Input will consist of a series of cases, each one in a line. A line describing a case contains p and q, two integer numbers separated by a space, with 10^20 &gt; p &gt; q &gt; 0.

</p><p><br>The end of the input is indicated by a line containing 0 0.

<br><br>
</p><h3>Output</h3>
<p>Cases must be analyzed in the order that are read from the input. Output for each case will consist of several lines. The first line indicates the case number, starting at 1, using the format:

</p><p><br>Case i:
<br>replacing i by the corresponding case number. The second line displays the input data in the
form p / q.

</p><p><br>The remaining lines must contain the continuous fraction corresponding to the rational
number, p
q , specified in the given input line. The continuous fraction must be printed accordingly to the following rules:

<br><br></p><ul>
<li>Horizontal bars are formed by sequences of dashes ‘-’.

<br><br></li><li>The width of each horizontal bar is exactly equal to the width of the denominator under it.

<br><br></li><li>Blank characters should be printed using periods ‘.’

<br><br></li><li>The number on a fraction numerator must be printed center justified. That is, the number of spaces at either side must be same, if possible; in other case, one more space must be added at the right side.
</li></ul>

<br>
<h3>Example</h3>

<br>
<pre><b>Input:</b>
75 34
65 60
0 0

<b>Output:</b>
Case 1:
75 / 34
..........1......
2.+.-------------
............1....
....4.+.---------
..............1..
........1.+.-----
................1
............5.+.-
................1
Case 2:
65 / 60
......1...
1.+.------
.........1
....11.+.-
.........1
</pre>