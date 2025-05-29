<p style="text-align: center;"><strong>Football Team</strong></p>
<p>A football team will be standing in rows to have a photograph taken. The location of each player will be given by two integers x and y, where y gives the number of the row, and x gives the distance of the player from the left edge of the row. The x values will be all different.</p>
<p>In order to make the photo more interesting, you're going to make sure players who are near each other have shirts of different colors. To do this, you set the following rule:<br> For each player P:</p>
<ul>
<li>The closest player to the right of P in the same row, if there is such a player, must have a different shirt color. </li>
<li>The closest player to the right of P in the previous row, if there is such a player, must have a different shirt color. </li>
<li>The closest player to the right of P in the next row, if there is such a player, must have a different shirt color. </li>
</ul>
<p>More formally, if there is a player at (x1,y1) and (x2,y2), where x1&lt;x2, then those two players must have different shirt colors if:</p>
<ul>
<li> y1 - 1 ¡Ü y2 ¡Ü y1 + 1, and </li>
<li> there is no x3 such that there is a player at (x3, y2) and x1 &lt; x3 &lt; x2. </li>
</ul>
<p>Find the minimum number of distinct shirt colors required so that this is possible.</p>
<p>Input</p>
<p>The first line of input contains a single integer <strong>T</strong>, the number of test cases. Each test case starts with a line that contains an integer <strong>N</strong>, the number of players, followed by <strong>N</strong> lines of the form</p>
<pre>x y</pre>
<p>each specifying the position of one player.</p>
<p>Output</p>
<p>For each test case, output</p>
<pre>Case #X: c</pre>
<p>where <strong>X</strong> is the test case number, starting from 1, and <strong>c</strong> is the minimum number of colors required.</p>
<p>Limits</p>
<p>1 ¡Ü <strong>T</strong> ¡Ü 100<br> 1 ¡Ü <strong>x</strong> ¡Ü 1000<br> The values of x will all be different.</p>
<p>Small dataset</p>
<p>1 ¡Ü <strong>y</strong> ¡Ü 15<br> 1 ¡Ü <strong>N</strong> ¡Ü 100</p>
<p>Large dataset</p>
<p>1 ¡Ü <strong>y</strong> ¡Ü 30<br> 1 ¡Ü <strong>N</strong> ¡Ü 1000</p>
<p>Sample</p>
<table style="width: 166px; height: 226px;" border="0">
<tbody>
<tr>
<td><br> <span>Input</span> <br>&nbsp;</td>
<td><br> <span>Output</span> <br>&nbsp;</td>
</tr>
<tr>
<td><code> 3<br> 3<br> 10 10<br> 8 15<br> 12 7<br> 5<br> 1 1<br> 2 1<br> 3 1<br> 4 1<br> 5 1<br> 3<br> 1 1<br> 2 2<br> 3 1<br> </code></td>
<td valign="top"><code> Case #1: 1<br> Case #2: 2<br> Case #3: 3<br> </code></td>
</tr>
</tbody>
</table>