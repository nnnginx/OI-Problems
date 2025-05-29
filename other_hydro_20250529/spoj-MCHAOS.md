<p>   </p>
<table style="width: 100%; background-color: #41bd46;" border="1">
<tbody>
<tr>
<td style="text-align: center;" width="50%"><a href="/problems/MCHAOS/en/">English</a></td>
<td style="text-align: center;" width="50%"><a href="/problems/MCHAOS/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>&nbsp;</p>
<p>Little Lovro likes to play games with words. During the last few weeks he realized that some words don't like each other.</p>
<p><br>The words A and B don't like each other if the word A is lexicographically before the word B, but the word B' is lexicographically before the word A', where X' stands for the word X reversed (if X="kamen" then X'="nemak"). For example, the words "lova" and "novac" like each other, but the words "aron" and "sunce" don't like each other.</p>
<p>Given some set of the words, we define&nbsp; the degree of chaos of the set as&nbsp; the number of pairs of different words that don't like each other.</p>
<p>Write a program that, given a set of words, finds the chaos degree for the set.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line of input contains an integer N, 2 ¡Ü N ¡Ü 100 000.</p>
<p>Each of the following N lines contains one word ¨C a sequence of at most 10 lowercase letters of the English alphabet ('a'-'z'). There will be no two identical words in the set.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>The first and only line of output should contain a single integer ¨C the chaos degree of the given set of words.</p>
<p><br>Note: use 64-bit signed integer type (int64 in Pascal, long long in C/C++).</p>
<p>&nbsp;</p>
<h3>Sample</h3>
<pre>input <br>&nbsp;<br>2 <br>lopta <br>kugla <br>&nbsp;<br>output <br>&nbsp;<br>0<br><br>input <br>&nbsp;<br>4 <br>lova <br>novac <br>aron <br>sunce <br>&nbsp;<br>output <br>&nbsp;<br>3<br><br>input <br>&nbsp;<br>14 <br>branimir <br>vladimir <br>tom <br>kruz <br>bred <br>pit <br>zemlja <br>nije <br>ravna <br>ploca <br>ko <br>je <br>zapalio <br>zito <br>&nbsp;<br>output <br>&nbsp;<br>48<br></pre>
<p> </p>