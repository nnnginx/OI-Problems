<p>In a far away country there are N cities, and every two of them are connected by a two-way direct airplane line. Gripped by the crisis, the airline company has decided to remove as many lines as possible.</p>
<p>The lines will be eliminated one by one. This elimination must not significantly affect the city connections, so when removing a line, it must belong to a cycle of length four. In other words, if the cities A, B, C, D are such that currently there are lines AB, BC, CD and DA, then we can remove any of these lines.</p>
<p>It is possible to prove that there must remain at least N lines at the end of the elimination process (i.e., that we are unable to remove more lines under the described conditions). You are not required to prove it, but to write a program that helps the airline company to remove a line by line until there are exactly N left.</p>
<h3>Input</h3>
<p>4 �� N �� 2000.</p>
<h3>Output</h3>
<p>Print one line of data for each airplane line you are removing.</p>
<p>In each of these lines, print the numbers A, B, C, D which represent the cities forming a cycle. These numbers indicate that you are removing the line AB.</p>
<h3>Example</h3>
<pre><table style="color: #000000; font-family: Arial; font-size: 12px;" border="0" cellspacing="2" cellpadding="0"><tbody><tr><td width="50%" valign="top"><span class="evl_tblzad_stitle" style="font-size: 12px; font-weight: bold;">input</span><br><pre class="evl_tblzad_stp" style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">4</pre>
<span class="evl_tblzad_stitle" style="font-size: 12px; font-weight: bold;">output</span><br>
<pre class="evl_tblzad_stp" style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">2 3 1 4
3 4 2 1</pre>
</td>
<td width="1px" bgcolor="#000000"><img src="./24125/file/8IztsLQC.png" alt="" width="1px"></td>
<td width="50%" valign="top"><span class="evl_tblzad_stitle" style="font-size: 12px; font-weight: bold;">input</span><br>
<pre class="evl_tblzad_stp" style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">5</pre>
<span class="evl_tblzad_stitle" style="font-size: 12px; font-weight: bold;">output</span><br>
<pre class="evl_tblzad_stp" style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">3 4 5 2
2 3 1 5
3 5 2 1
2 4 1 5
4 5 2 1</pre>
</td>
</tr>
</tbody>
</table>
</pre>