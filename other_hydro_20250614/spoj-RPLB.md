<p>Teresa picked up enough strawberries, now she wants to pick blueberries from the magical blueberry bush from Rainbowland.</p>
<p>Knowing her previous experience with the strawberries, Teresa wants to pick up the blueberries in a way that she may not exceed the limit proposed.</p>
<p>When picking the blueberries, she noticed that if she pick from the bush i, she couldn't pick the blueberries at the bush i+1 (some sort of magic in rainbowland).</p>
<p>Worried about this, Teresa wants to know the maximum blueberries she can pick, given the number of bushes and the number of blueberries in each bush.</p>

<h3>Input</h3>
<p>Will contain an integer T, then, T cases will follow, each case starts with a number N and K, being N the number of bushes and K the number of blueberries Teresa will pick as maximum, the next line contains N integers, each one representing the blueberries there is on the i-th bush.</p>

<h3>Output</h3>
<p>You will output for each test case the string: <tt>¡°Scenario #i: ¡°</tt> where i is the test case you are analyzing, then, an integer denoting the maximum number of blueberries you can grab.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
5 100
50 10 20 30 40
5 87
21 45 30 12 14

<strong>Output:</strong>
Scenario #1: 90
Scenario #2: 65</pre>

<!--
<center>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
  <td width="120px"><p align="CENTER"><strong>INPUT</strong></p></td>
  <td width="120px"><p align="CENTER"><strong>OUTPUT</strong></p></td>
</tr>
<tr>
  <td valign="top">
<pre>
2
5 100
50 10 20 30 40
5 87
21 45 30 12 14</pre>
  </td>
  <td valign="top">
<pre>Scenario #1: 90
Scenario #2: 65</pre>
  </td>
</tr>
</tbody>
</table>
</center>

-->
<!-- <p>¡°Blank line between test cases for clarification and separation¡±</p> -->

<h4>Output explanation (first scenario)</h4>
<p>Teresa picks the 1<sup>st</sup> blueberry bush (50), she cannot pick the 2<sup>nd</sup>, she decides not to pick until the 5<sup>th</sup> one where she picks the ¡°40¡± blueberry, she could pick the 3<sup>rd</sup> bush, but she would exceed the limit (100).</p>

<h4>Output explanation (second scenario)</h4>
<p>Teresa picks the 1<sup>st</sup>, the 3<sup>rd</sup> and the 5<sup>th</sup> bush, total of (21+30+14 = 65) blueberries</p>

<h3>CONSTRAINTS</h3>
<p>
1 &lt;= N &lt;= 1000<br>
1 &lt;= K &lt;= 1000
</p>