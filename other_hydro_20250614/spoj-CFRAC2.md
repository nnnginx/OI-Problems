<p>A simple continuous fraction has the form:
</p><p><br>
</p><center><img src="/content/steinersp:cfrac.jpg" alt="subir imagenes" border="0"></center>

<p><br><br>where the ai’s are integer numbers.

</p><p><br>The previous continuous fraction could be noted as [a1, a2, . . . , an]. It is not difficult to show that any rational number p / q , with integers p &gt; q &gt; 0, can be represented in a unique way by a simple continuous fraction with n terms, such that p / q = [a1, a2, . . . , an−1, 1], where n and the ai’s are positive natural numbers.

</p><p><br>Now given a simple continuous fraction, your task is to calculate a rational number which the continuous fraction most corresponds to it. 

</p><p><br>
</p><h3>Input</h3>
<p>Input for each case will consist of several lines. The first line is two integer m and n,which describe a char martrix,then followed m lines,each line cantain n chars.
The char martrix describe a continuous fraction The continuous fraction is described by the following rules:

</p><p><br>
</p><li>Horizontal bars are formed by sequences of dashes `-'.

<p>
<br></p></li><li>The width of each horizontal bar is exactly equal to the width of the denominator under it.
<br></li><li>Blank characters should be printed using periods `.'

<p>
<br></p></li><li>The number on a fraction numerator must be printed center justified. That is, the number of spaces at either side must be same, if possible; in other case, one more space must be added at the right side.
<p></p>

<p>The end of the input is indicated by a line containing 0 0. </p>

<h3>Output</h3>
<p>Output will consist of a series of cases, each one in a line corresponding to the input case. A line describing a case contains p and q, two integer numbers separated by a space, and you can assume that 10^20 &gt; p &gt; q &gt; 0. 

</p><h3>Example</h3>

<pre><b>Input:</b>
9 17
..........1......
2.+.-------------
............1....
....4.+.---------
..............1..
........1.+.-----
................1
............5.+.-
................1
5 10
......1...
1.+.------
.........1
....11.+.-
.........1
0 0

<b>Output:</b>
75 34
13 12
</pre>

</li>