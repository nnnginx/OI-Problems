<p>There are N hotels along the beautiful Adriatic coast. Each hotel has its value in Euros.</p>
<p>Sroljo has won M Euros on the lottery. Now he wants to buy a sequence of consecutive hotels, such that the sum of the values of these consecutive hotels is as great as possible - but not greater than M.</p>
<p>You are to calculate this greatest possible total value.</p>
<h3>Input</h3>
<p>In the first line of the input there are integers N and M (1 �� N �� 300 000, 1 �� M &lt; 2<sup>31</sup>).</p>
<p>In the next line there are N natural numbers less than 10<sup>6</sup>, representing the hotel values in the order they lie along the coast.</p>
<h3>Output</h3>
<p>Print the required number (it will be greater than 0 in all of the test data).</p>
<h3>Example</h3>
<table style="color: #000000; font-family: Arial; font-size: 12px;" border="0" cellspacing="2" cellpadding="0">
<tbody>
<tr>
<td width="50%" valign="top"><span style="font-size: 12px; font-weight: bold;">input</span><br>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">5 12
2 1 3 4 5</pre>
<span style="font-size: 12px; font-weight: bold;">output</span><br>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">12</pre>
</td>
<td width="1px" bgcolor="#000000"><img src="./22799/file/xfU2fjLe.png" alt="" width="1px"></td>
<td width="50%" valign="top"><span style="font-size: 12px; font-weight: bold;">input</span><br>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">4 9
7 3 5 6</pre>
<span style="font-size: 12px; font-weight: bold;">output</span><br>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">8</pre>
</td>
</tr>
</tbody>
</table>