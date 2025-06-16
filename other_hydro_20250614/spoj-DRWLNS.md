<pre><span style="white-space: normal;"><span style="font-size: medium;"><p>John is a bit upset now. Today was his chemistry central viva and it did not go very well. So to cheer up he bought a notebook, a pencil and an eraser.</p>
<p>In the note book there are N points drawn in a row. The points are numbered from 1 to N serially.</p>
<p>Now, John decided to do a strange thing with those points.</p>
<p>At each moment, John puts his pencil or eraser at a point A and drags it to point B. As a result, some line segments may be created.</p>
<p>And then, Sometimes he stops and thinks of a point C and tries to find out if point C is on a line segment or not.</p>
<p>You have to solve a similar problem.</p>
<p>&nbsp;</p>
<p><strong><span style="text-decoration: underline;">INPUT:</span></strong></p>
<p>First line of the input will contain two integers N (1&lt;=n&lt;=10<sup>9</sup>) and M (1&lt;=M&lt;=10<sup>5</sup>) where N denotes number of points and M denotes number of queries.</p>
<p>Then M line follows. Each line contains a query.</p>
<p>Each query will be one of the following forms:</p>
<p><strong>0 A B</strong>: which means an eraser has been dragged from point A to point B.</p>
<p><strong>1 A B:&nbsp;</strong>which means a pencil has been dragged from point A to point B.</p>
<p><strong>2 C:&nbsp;</strong>which means you are asked to answer the state of point C. There will be at least one query of this type.</p>
<p>(It is guaranteed that A&lt;=B and 1&lt;=A, B, C&lt;=N)</p>
<p><strong><span style="text-decoration: underline;">OUTPUT:</span></strong></p>
<p>For each query of the form&nbsp;<strong>¡°2 C¡±,</strong>&nbsp;print a single line.If point C is&nbsp;<strong>NOT&nbsp;</strong>on any line segment then print -1.</p>
<p>Otherwise, print the start and end point of the segment.</p>
<p>See sample input/ sample output and explanation for details.</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="319" valign="top">
<p><strong>Sample   Input</strong></p>
</td>
<td width="319" valign="top">
<p><strong>Sample   Output</strong></p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p>25 14</p>
<p>2 10</p>
<p>1 20 25</p>
<p>1 9 13</p>
<p>2 12</p>
<p>2 7</p>
<p>1 11 21</p>
<p>2 15</p>
<p>0 17 20</p>
<p>0 22 25</p>
<p>2 21</p>
<p>2 5</p>
<p>1 1 8</p>
<p>2 12</p>
<p>2 4</p>
</td>
<td width="319" valign="top">
<p>-1</p>
<p>9 13</p>
<p>-1</p>
<p>9 25</p>
<p>21 21</p>
<p>-1</p>
<p>9 16</p>
<p>1 8</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><strong><span style="text-decoration: underline;">Explanation:</span></strong></p>
<p>In the 1<sup>st</sup>&nbsp;query, there are no line segments. So point 10 is not on any segment.</p>
<p>After 2<sup>nd</sup>&nbsp;query, there is 1 line segment: [20, 25].</p>
<p>After 3rd&nbsp;query, there are 2 line segments:&nbsp; [9, 13], [20, 25].</p>
<p>In the 4<sup>th&nbsp;</sup>query, point 12 is on [9, 13] segment.</p>
<p>In the 5<sup>th</sup>&nbsp;query, point 7 is not on any segment.</p>
<p>After 6<sup>th</sup>&nbsp;query, there is 1 line segment [9, 25]. ([9, 13], [11, 21] and [20, 25] segments will merge into only 1 segment).</p>
<p>In the 7<sup>th</sup>&nbsp;query, point 15 is on [9, 25] segment.</p>
<p>After 9<sup>th</sup>&nbsp;query there are 2 segments: [9, 16] and [21, 21].</p>
<p>In the 10<sup>th</sup>&nbsp;query, point 21 is on [21, 21] segment.</p>
<p>In the 11<sup>th</sup>&nbsp;query, point 5 is not on any segment.</p>
<p>After 12<sup>th</sup>&nbsp;query there are 3 segments: [1,8],[9, 16] and [21, 21].</p>
<p>In the 13<sup>th</sup>&nbsp;query, point 13 is on [9, 16] segment.</p>
<p>In the 14<sup>th</sup>&nbsp;query, point 4 is on [1, 8] segment.</p>
<p>&nbsp;</p></span></span></pre>