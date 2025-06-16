<h3>Problem Statement</h3>

<p>
Given two string <strong>S</strong> and <strong>T</strong>. You can delete a character from <strong>S</strong> with cost 15 and a Character <strong>T</strong> with cost 30. Your goal is to make the string equal (same). It is not mandatory to delete character.</p>

<p>For example: S = <strong>aXb</strong> and T = <strong>Yab</strong>. Now, if we delete X from S and Y from T, then total cost = 15 + 30 = 45. 
And S and T will become <strong>ab</strong>.
</p>

<p>Another example: S = <strong>ab </strong>, T = <strong>cd</strong>, Now total cost = 15 + 15 + 30 + 30 = 90.</p>
<p>Another example: S = <strong>abcd</strong>, T = <strong>acdb</strong>, Now total cost = 15 + 30 = 45.</p>

<h3>Input</h3>
<p>Input consists of pairs of lines. The first line of a pair contains the first string <strong>S</strong> and the second line contains the second string <strong>T</strong>. Each string is on a separate line and consists of at most 1,000 characters . The end of input occurs when the first sequence starts with an "<code>#</code>" character (without the quotes).</p>

<h3>Output</h3>
<p>For each subsequent pair of input lines, output a line containing one integer number which the minimum cost to make the string equal (same).</p>

<h3>Sample Input/Output</h3>
<table style="width: 656px;" border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="328" valign="top">
<p style="text-align: center;"><strong>Sample Input</strong></p>
</td>
<td width="328" valign="top">
<p style="text-align: center;"><strong>Sample Output</strong></p>
</td>
</tr>
<tr>
<td width="328" valign="top">
<pre>axb
yab
ab
cd
ko
p
abcd
acdb
#</pre>
</td>
<td width="328" valign="top">
<pre>45
90
60
45
</pre>
</td>
</tr>
</tbody>
</table>

<p><br></p><p>___________________________________________________________________________________________________________<br><strong>Problem Setter: Shipu Ahamed, Dept. of CSE </strong></p><p><strong><em>Bangladesh University of Business and Technology (BUBT)</em></strong></p>