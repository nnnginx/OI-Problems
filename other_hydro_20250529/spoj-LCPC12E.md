<h3>Description</h3>

<p>Hundreds of years ago Johnny's father had a great kingdom. Before his death he divided his kingdom between his sons (Johnny and Johnny's brother). Johnny's brother took part of the kingdom with a circular shape with radius <strong><em>R</em></strong>.&nbsp; Jonny took part of kingdom of squared shape with side length <strong><em>L</em></strong>. As Johnny was jealous from his brother after his father's death, he decided to extend his kingdom to be a circle such that the corners of the square lies exactly on the border of the circle. A problem might occur that Johnny could steal some land from his brother, and that could wage a huge war between the two brothers. So Johnny decided to convince his brother to build a wall separating between the two kingdoms. The wall should be connecting the two intersection points between the two circles. You are to estimate the length of this wall.</p>
<p><img src="./23150/file/5wHLdc8J.png" alt="" width="425" height="235"></p>

<h3>Input Format</h3>
<p>The first line of input contains an integer <strong><em>T</em></strong>, the number of test cases. <strong><em>T</em></strong> test cases follow, the first line of each test case contains 6 floating point numbers; 2 numbers denoting the center of Johnny's brother kingdom, another 2 for the center of Johnny's kingdom, <strong><em>R</em></strong> the radius of Johnny's brother kingdom <strong><em>A</em></strong>, and <strong><em>L</em></strong> the side length of the square of Johnny's kingdom. It¡¯s guaranteed that both kingdoms don¡¯t share any lands originally. Also after kingdom <strong><em>B</em></strong> is extended, it¡¯s guaranteed that the intersection area will not cover Johnny's brother kingdom completely. The absolute value for all decimal numbers will be less than 10<sup>9</sup>.</p>

<h3>Output Format</h3>
<p>There should be <strong><em>T</em></strong> lines, containing the following format.</p>
<p><strong><em>k. S</em></strong></p>
<p>Where <strong><em>k</em></strong> is the test case number (starting at 1), a single period, a single space and <strong><em>S</em></strong> represent a decimal number with exactly 3 digits after the decimal point representing the wall length. If there¡¯s no possibility of war, print ¡°<strong><em>No problem</em></strong>¡±.</p>

<table style="width: 100%;" border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td valign="top">
<p><strong>Sample Input</strong></p>
</td>
<td valign="top">
<p><strong>Sample Output</strong></p>
</td>
</tr>
<tr>
<td valign="top">
<pre>3
0.0 0.0 10.0 0 3 3
0.0 0.0 4.121 0 3 3
-1 3 1 -1 2 7.071</pre>
</td>
<td valign="top">
<pre>1. No problem
2. 2.971
3. 3.994</pre>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>