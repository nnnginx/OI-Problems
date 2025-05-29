<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/DQUERY/en/">English</a></td>
<td width="50%"><a href="/problems/DQUERY/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Given a sequence of n numbers a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>n</sub> and a number of d-queries. A d-query is a pair (i, j) (1 ¡Ü i ¡Ü j ¡Ü n). For each d-query (i, j), you have to return the number of distinct elements in the subsequence a<sub>i</sub>, a<sub>i+1</sub>, ..., a<sub>j</sub>.</p>
<h3>Input</h3>
<ul>
<li>Line 1: n (1 ¡Ü n ¡Ü 30000).</li>
<li>Line 2: n numbers a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>n</sub> (1 ¡Ü a<sub>i</sub> ¡Ü 10<sup>6</sup>).</li>
<li>Line 3: q (1 ¡Ü q ¡Ü 200000), the number of d-queries.</li>
<li>In the next q lines, each line contains 2 numbers i, j representing a d-query (1 ¡Ü i ¡Ü j ¡Ü n).</li>
</ul>
<h3>Output</h3>
<ul>
<li>For each d-query (i, j), print the number of distinct elements in the subsequence a<sub>i</sub>, a<sub>i+1</sub>, ..., a<sub>j</sub> in a single line.
<p>&nbsp;</p>
</li>
</ul>
<h3>Example</h3>
<pre><strong>Input</strong>
5
1 1 2 1 3
3
1 5
2 4
3 5

<strong>Output</strong>
3
2
3 
</pre>
<p> </p>