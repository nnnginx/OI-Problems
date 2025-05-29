<p align="center"><strong>8. Build the Tower</strong></p>
<p>The president of Yanyang University has decided to build a new tower in front of the auditorium and has invited the students of SCE to help with the project. The tower is one of a kind and is made up of N cuboids one over the other. Each cuboid has a height of 1 unit and the length and breadth of a cuboid is equal. The top most cuboid¡¯s length is 1 unit. The cuboid below it has a length of 2. All the cuboids below it have their lengths equal to the sum of the lengths of the 2 cuboids above it.</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="102" valign="top">
<p align="center">Cuboid</p>
</td>
<td width="76" valign="top">
<p align="center">Length</p>
</td>
<td width="94" valign="top">
<p align="center">Breadth</p>
</td>
<td width="76" valign="top">
<p align="center">Height</p>
</td>
</tr>
<tr>
<td width="102" valign="top">
<p align="center">1</p>
</td>
<td width="76" valign="top">
<p align="center">1</p>
</td>
<td width="94" valign="top">
<p align="center">1</p>
</td>
<td width="76" valign="top">
<p align="center">1</p>
</td>
</tr>
<tr>
<td width="102" valign="top">
<p align="center">2</p>
</td>
<td width="76" valign="top">
<p align="center">2</p>
</td>
<td width="94" valign="top">
<p align="center">2</p>
</td>
<td width="76" valign="top">
<p align="center">1</p>
</td>
</tr>
<tr>
<td width="102" valign="top">
<p align="center">3</p>
</td>
<td width="76" valign="top">
<p align="center">3</p>
</td>
<td width="94" valign="top">
<p align="center">3</p>
</td>
<td width="76" valign="top">
<p align="center">1</p>
</td>
</tr>
<tr>
<td width="102" valign="top">
<p align="center">4</p>
</td>
<td width="76" valign="top">
<p align="center">5</p>
</td>
<td width="94" valign="top">
<p align="center">5</p>
</td>
<td width="76" valign="top">
<p align="center">1</p>
</td>
</tr>
<tr>
<td width="102" valign="top">
<p align="center">5</p>
</td>
<td width="76" valign="top">
<p align="center">8</p>
</td>
<td width="94" valign="top">
<p align="center">8</p>
</td>
<td width="76" valign="top">
<p align="center">1</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>As a token of appreciation the president has decided to give SCE a grant of</p>
<p align="center"><strong>$ ((Volume of Tower) % 1000000007)</strong></p>
<p>Your task is to calculate the amount of grant received by SCE for a given value of N.</p>

<h3>Input</h3>
<p>The first line contains the number of test cases (T) followed by T lines each containing a single integer N.</p>

<h3>Output</h3>
<p>For each test case output the grant that SCE receives for building the tower.</p>

<h3>Constraints</h3>
<p>T &lt;= 20, N &lt;= 10^18</p>

<h3>Example</h3>
<p><strong>Sample Input</strong></p>
<pre>2
5
10</pre>
<p><strong>Sample Output</strong></p>
<pre>$103
$12815</pre>