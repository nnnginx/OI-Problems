<p>A group of people is trying to beat the world record for the largest number of people having lunch at the same time. In order achieve this goal, they are using the country's	 largest bridge and they have decided to arrange the tables following the shape of the letter 'S'.</p>
<p>The table layout can be described by 4 integers: <strong>NH</strong>, <strong>NV</strong>, <strong>H</strong> and <strong>V</strong>. The two first integers, <strong>NH</strong> and <strong>NV</strong>, represent respectively the number or rows and number of columns in the layout. The last two integers represent respectively the number of tables in each row and column. For a given layout, the tables are numbered consecutively, starting with table #1 in the top-right corner. The following figure illustrates several possible layouts:</p>
<p><img src="../../content/mogers:wrlunch_c2" alt="" width="600" height="286"></p>
<p>Thousands of groups of people are expected to come, and the organizers have to define where to seat everyone. Each group needs a certain number of tables and they do not share tables with other groups. Furthermore, a group wants their tables to be together and not split among rows and columns, that is, they want a set of consecutive tables either on the same row or on the same column. If this condition cannot be met, the group prefers to go away and have lunch at another place. The groups also enjoy having some privacy and prefer unoccupied adjacent tables, that is, no one at the table exactly before the first table of the group, and no one at the table exactly after the last table of the group. If this happens, we say that the group found a <strong>private</strong> place.</p>
<p>Whenever a group arrives, the organization must decide where to seat that group based solely on the table occupation at the moment, without taking into account further groups that may be coming. Since a group will always be seated on consecutive tables, the position of a group can be defined by the index of the first table of the group. So, when a group arrive, the organization wants the following:</p>
<ul>
<li>If there is a suitable private place for the group, then choose the lowest possible index guaranteeing privacy;</li>
<li>If no privacy can be ensured, but there is space for the group, then choose the lowest possible index with space for the entire group;</li>
<li>If there is no space available on a single row or column where the group would fit, then the organizers must send the group away.</li>
</ul>
<p>An example would be the following. Imagine a layout with <strong>NH</strong>=3,<strong> NV</strong>=2, <strong>H</strong>=5 and <strong>V</strong>=3 (the first layout give on the figure above). And now imagine that groups needing 5, 2, 3, 5, 4 and 2 tables arrive, in that order. This is what happens:</p>
<table border="0" cellspacing="1" cellpadding="2" bgcolor="#888888">
<tbody>
<tr bgcolor="white">
<td><img src="../../content/mogers:wrlunch_c3-1" alt="" width="108" height="109"></td>
<td>In the beginning all tables are empty</td>
</tr>
<tr bgcolor="white">
<td width="320"><img src="../../content/mogers:wrlunch_c3-2" alt="" width="104" height="105"> <img src="../../content/mogers:wrlunch_c3-3" alt="" width="105" height="109"> <img src="../../content/mogers:wrlunch_c3-4" alt="" width="101" height="106"></td>
<td>Group 1 needs 5 tables. It is put on index 1.<br> Group 2 needs 2 tables. It is put on index 7.<br> Group 3 needs 3 tables. It is put on index 11.<br> Group 4 needs 5 tables. No position is available.<br></td>
</tr>
<tr bgcolor="white">
<td><img src="../../content/mogers:wrlunch_c3-5" alt="" width="106" height="106"> <img src="../../content/mogers:wrlunch_c3-6" alt="" width="102" height="105"></td>
<td>Group 5 needs 4 tables. It is put on index 14 (with no privacy).<br> Group 6 needs 2 tables. It is put on index 9 (with no privacy).<br></td>
</tr>
</tbody>
</table>
<p>Can you help the organizers on this task?</p>
<h2>The Problem</h2>
<p>Given a table layout (number of rows, columns and number of tables per row and column) and the description of groups arriving (specifying number of tables needed per group), your task is to calculate where each group should be seated following the rules described above.</p>
<h2>Input</h2>
<p>The first line contains 5 integers <strong>NH NV H V N</strong>, separated by single spaces. <strong>NH</strong> and <strong>NV</strong> indicate respectively the number of rows and columns of the table layout. <strong>H</strong> and <strong>V</strong> indicate respectively the number of tables per row and column. <strong>N</strong> indicates the number of groups arriving.</p>
<p>Then come <strong>N</strong> lines, each one indicating <strong>G<sub>i</sub></strong>, the number of tables the <em>i</em>-th group needs. These lines come in order of arrival of the groups.</p>
<h2>Output</h2>
<p>The output should have exactly <strong>N</strong> lines, each one indicating where the respective group should seat. If there is a suitable position, the line should contain an integer indicating the index of the first table of the group. If no position is available, the line should contain the string <tt>"no"</tt>, without the quotes.</p>
<h2>Restrictions</h2>
<p>The following limits are guaranteed for all the test cases that will be used for evaluating your program:</p>
<table border="0">
<tbody>
<tr>
<td><strong>1 �� NH �� 10&nbsp;000</strong></td>
<td>&nbsp;</td>
<td>Number of rows</td>
</tr>
<tr>
<td><strong>NH-1 �� NV �� NH</strong></td>
<td>&nbsp;</td>
<td>Number of columns</td>
</tr>
<tr>
<td><strong>3 �� H,V �� 1&nbsp;000</strong></td>
<td>&nbsp;</td>
<td>Number of tables in each row/column</td>
</tr>
<tr>
<td><strong>1 �� N �� 50&nbsp;000</strong></td>
<td>&nbsp;</td>
<td>Number of groups</td>
</tr>
<tr>
<td><strong>1 �� G<sub>i</sub> �� 1&nbsp;000</strong></td>
<td>&nbsp;</td>
<td>Number of tables each group needs</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<table border="0">
<tbody>
<tr>
<td valign="top">
<h2>Example Input 1</h2>
<pre>3 2 5 3 6
5
2
3
5
4
2
</pre>
<h2>Example Output 1</h2>
<pre>1
7
11
no
14
9
</pre>
<h2>Input Explanation 1</h2>
<p>It is the example given before in the problem statement.</p>
</td>
<td width="50">&nbsp;</td>
<td valign="top">
<h2>Example Input 2</h2>
<pre>2 2 3 3 3
3
3
1
</pre>
<h2>Example Output 2</h2>
<pre>1
5
9</pre>
<h2>Input Explanation 2</h2>
<p>In the end the tables would look like this:<br> <img src="../../content/mogers:wrlunch_c4" alt="" width="73" height="120"></p>
</td>
</tr>
</tbody>
</table>
<p>A few notes:</p>
<ul>
<li>This is the first problem I add to SPOJ, hope you like it :)</li>
<li>The time limit is at least 6x the runtime of my C++ solution with no low-level optimizations or fast input/output. I have a Java solution passing within these time limits.</li>
<li>I'm not proficient enough in languages like Python to ensure the time limit is ok for those languages. I can increase the limits if needed. </li>
</ul>