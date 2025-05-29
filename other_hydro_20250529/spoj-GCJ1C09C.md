<table border="0">
<tbody id="dsb-input-form-table2">
<tr>
<td><br></td>
<td>&nbsp;</td>
</tr>
</tbody>
</table>
<div id="dsb-problem-content-div2" style="text-align: justify;">
<p><strong>Problem</strong></p>
<p>In a kingdom there are prison cells (numbered 1 to <strong>P</strong>) built to form a straight line segment. Cells number <strong>i</strong> and <strong>i+1</strong> are adjacent, and prisoners in adjacent cells are called "neighbours."    A wall with a window separates adjacent cells, and neighbours can  communicate through that window.</p>
<p>All prisoners live in peace until a prisoner is released.  When that  happens, the released prisoner's neighbours find out, and each  communicates this to his other neighbour.  That prisoner passes it on to  <em>his</em> other neighbour, and so on until they reach a prisoner with no other neighbour (because he is in cell 1, or in cell <strong>P</strong>,  or the other adjacent cell is empty).  A prisoner who discovers that  another prisoner has been released will angrily break everything in his  cell, unless he is bribed with a gold coin. So, after releasing a  prisoner in cell <strong>A</strong>, all prisoners housed on either side of cell <strong>A</strong> - until cell 1, cell <strong>P</strong> or an empty cell - need to be bribed.</p>
<p>Assume that each prison cell is initially occupied by exactly one  prisoner, and that only one prisoner can be released per day. Given the  list of <strong>Q</strong> prisoners to be released in <strong>Q</strong> days, find the minimum total number of gold coins needed as bribes if the prisoners may be released in any order.</p>
<p>Note that each bribe only has an effect for one day. If a prisoner who  was bribed yesterday hears about another released prisoner today, then  he needs to be bribed again.</p>
<p><strong>Input</strong></p>
<p>The first line of input gives the number of cases, <strong>N</strong>. <strong>N</strong> test cases follow. Each case consists of 2 lines. The first line is formatted as</p>
<p>P Q</p>
where <strong>P</strong> is the number of prison cells and <strong>Q</strong> is the number of prisoners to be released.<br> This will be followed by a line with <strong>Q</strong> distinct cell numbers (of the prisoners to be released), space separated, sorted in ascending order.
<p><strong>Output</strong></p>
<p>For each test case, output one line in the format</p>
<pre>Case #X: C</pre>
where <strong>X</strong> is the case number, starting from 1, and <strong>C</strong> is the minimum number of gold coins needed as bribes.
<p><strong>Limits</strong></p>
<p>1 �� <strong>N</strong> �� 100<br> <strong>Q</strong> �� <strong>P</strong><br> Each cell number is between 1 and <strong>P</strong>, inclusive.</p>
<p>Large dataset</p>
<p>1 �� <strong>P</strong> �� 10000<br> 1 �� <strong>Q</strong> �� 100</p>
<p><strong>Sample</strong></p>
<div>
<table border="0">
<tbody>
<tr>
<td><br> <span>Input</span> <br>&nbsp;</td>
<td><br> <span>Output</span> <br>&nbsp;</td>
</tr>
<tr>
<td><code> 2<br> 8 1<br> 3<br> 20 3<br> 3 6 14<br> </code></td>
<td><code> Case #1: 7<br> Case #2: 35<br> </code></td>
</tr>
</tbody>
</table>
</div>
<p>Note</p>
<p>In the second sample case, you first release the person in cell 14, then  cell 6, then cell 3. The number of gold coins needed is 19 + 12 + 4 =  35. If you instead release  the person in cell 6 first, the cost will be  19 + 4 + 13 = 36.</p>
</div>