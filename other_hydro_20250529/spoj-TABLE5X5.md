<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/TABLE5X5/en/">English</a></td>
<td width="50%"><a href="/problems/TABLE5X5/vn/">Tiếng Việt</a></td> 
</tr></tbody></table>

<p>Having a 5x5-table, we make a right-table by filling letters from 'A'..'Y' into the table satisfying:
</p><ul>
<li>Each letter is used exactly one time.</li>
<li>The letters is ascending on every row.</li>
<li>The letters is ascending on every column.</li>
</ul>
<p>Each right-table is described by a 25-length string, see the example below for detail:
</p><p>The right-table:
</p><table>
<tbody><tr><td>A</td><td>B</td><td>C</td><td>D</td><td>E</td></tr>
<tr><td>F</td><td>G</td><td>H</td><td>I</td><td>J</td></tr>
<tr><td>K</td><td>L</td><td>M</td><td>N</td><td>O</td></tr>
<tr><td>P</td><td>Q</td><td>R</td><td>S</td><td>T</td></tr>
<tr><td>U</td><td>V</td><td>W</td><td>X</td><td>Y</td></tr>
</tbody></table>
<p>is described by the string "ABCDEFGHIJKLMNOPQRSTUVWXY".
</p><p>All descriptions are sorted ascending (following the dictionary order) and numbered from 1.
</p><p></p><h3>Task</h3>
<ul>
<li>Give an order, find the right description.</li>
<li>Give a description, find the right order.</li>
</ul>
<h3>Input</h3>
<p>
</p><ul>
<li>The first line contains a number (an order).</li>
<li>The second line contains a description.</li>
</ul>
<h3>Output</h3>
<p>
</p><ul>
<li>The first line contains the 25-length string desribing the order given.</li>
<li>The second line contains the order of the given description.</li>
</ul>
<h3>Example</h3>

<pre><b>Input:</b>
1
ABCDEFGHIJKLMNOPQRSTUVWXY

<b>Output:</b>
ABCDEFGHIJKLMNOPQRSTUVWXY
1
</pre>