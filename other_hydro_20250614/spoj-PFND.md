<p>Rahat lives in a strange country. Name of the cities of this country are also strange. Instead of traditional naming, here, cities are named by number like 1, 2, 3 ��..<strong>N</strong>. Cities are named according to their size. That is, city <strong>1</strong> is the smallest city, city <strong>2 </strong>is 2<sup>nd</sup> smallest��. city <strong>N </strong>is the largest city of the country.</p>
<p>People of the country are very concerned about traffic. To avoid collision and jam, every road is one directional. Rule of visiting from one city to another are:</p>
<ul>
<li>When visiting from a city to a <strong>larger</strong> city, you must have to journey through bus.</li>
<li>When visiting from a city to a <strong>smaller </strong>city, you must have to journey through train.</li>
</ul>
<p>Rahat lives in city <strong>1</strong>. He wants to go in city <strong>N</strong>. As he likes journey very much, he wants to know, in how many ways he can complete his journey.</p>
<p>He dislikes riding on train. So he will <strong>not</strong> ride on train during his journey.</p>
<h3>Input</h3>
<p>Input set starts with an integer (<strong>T</strong>&lt;=101), denoting the test case. Then <strong>T </strong>test case follows.</p>
<p>Each case starts with two integer (1 &lt;= <strong>N</strong> &lt;= 10^5, 0&lt;=<strong>M</strong>&lt;=MIN (10^5, (N*(N-1))/2)), where <strong>N</strong> denotes number of cities and <strong>M</strong> denotes number of roads in that city. Then <strong>M</strong> lines follow. Each line denotes two integers (1&lt;= <strong>u, v</strong> &lt;= <strong>N, u != v</strong>) which indicates there is a road between <strong>u</strong> and <strong>v</strong> for bus transportation.</p>
<h3>Output</h3>
<p>For each case, print total way Rahat can make to arrive on city <strong>N</strong>. As the answer can be very big, print the answer modulo 1000000007. For correct format, look at the sample output.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>1</p><p>4 3</p><p>1 2</p><p>2 3</p><p>3 4</p>
<strong>Output:</strong>
<table style="width: 641px;" border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="320" valign="top">
<p>Case 1: 1</p>
</td>
</tr>
</tbody>
</table></pre>