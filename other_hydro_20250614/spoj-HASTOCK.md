<p style="text-align: center;"><strong>B - Stock Charts</strong></p>
<p>You're in the middle of writing your newspaper's end-of-year economics summary, and you've decided that you want to show a number of charts to demonstrate how different stocks have performed over the course of the last year. You've already decided that you want to show the price of <strong>n</strong> different stocks, all at the same <strong>k</strong> points of the year.</p>
<p>A <em>simple chart</em> of one stock's price would draw lines between the points (0, price<sub>0</sub>), (1, price<sub>1</sub>), ... , (k-1, price<sub>k-1</sub>), where price<sub>i</sub> is the price of the stock at the <em>i</em>th point in time.</p>
<p>In order to save space, you have invented the concept of an <em>overlaid chart</em>. An overlaid chart is the combination of one or more simple charts, and shows the prices of multiple stocks (simply drawing a line for each one). In order to avoid confusion between the stocks shown in a chart, the lines in an overlaid chart may not cross or touch.</p>
<p>Given a list of <em>n</em> stocks' prices at each of <em>k</em> time points, determine the minimum number of overlaid charts you need to show all of the stocks' prices.</p>
<p>Input</p>
<p>The first line of input will contain a single integer <strong>T</strong>, the number of test cases.  After this will follow <strong>T</strong> test cases on different lines, each of the form:</p>
<pre>n k<br>price<sub>0,0</sub> price<sub>0,1</sub> ... price<sub>0,k-1</sub><br>price<sub>1,0</sub> price<sub>1,1</sub> ... price<sub>1,k-1</sub><br>...<br>price<sub>n-1,0</sub> price<sub>n-1,1</sub> ... price<sub>n-1,k-1</sub><br></pre>
<p>Where price<sub>i,j</sub> is an integer, the price of the <em>i</em>th stock at time <em>j</em>.</p>
<p>Output</p>
<p>For each test case, a single line containing "Case #X: Y", where <em>X</em> is the number of the test-case (1-indexed) and <em>Y</em> is the minimum number of overlaid charts needed to show the prices of all of the stocks.</p>
<p>Limits</p>
<p>1 �� <strong>T</strong> �� 100<br> 2 �� <strong>k</strong> �� 25<br> 0 �� price<sub>i,j</sub> �� 1000000</p>
<p>1 �� <strong>n</strong> �� 16</p>
<p>Sample</p>
<table style="width: 158px; height: 226px;" border="0">
<tbody>
<tr>
<td><br> <span>Input</span> <br>&nbsp;</td>
<td><br> <span>Output</span> <br>&nbsp;</td>
</tr>
<tr>
<td><code> 3<br> 3 4<br> 1 2 3 4<br> 2 3 4 6<br> 6 5 4 3<br> 3 3<br> 5 5 5<br> 4 4 6<br> 4 5 4<br> 5 2<br> 1 1<br> 2 2<br> 5 4<br> 4 4<br> 4 1<br> </code></td>
<td valign="top"><code> Case #1: 2<br> Case #2: 3<br> Case #3: 2</code></td>
</tr>
</tbody>
</table>