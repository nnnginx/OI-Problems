<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/ORDERSET/en/">English</a></td>
<td width="50%"><a href="/problems/ORDERSET/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>In this problem, you have to maintain a dynamic set of   numbers which support the two fundamental operations</p>
<ul>
<li>INSERT(S,x): if x is not in S, insert x into S</li>
<li>DELETE(S,x): if x is in S, delete x from S</li>
</ul>
<p>and the two type of queries</p>
<ul>
<li>K-TH(S) : return the k-th smallest element of S</li>
<li>COUNT(S,x): return the number of elements of S smaller   than x</li>
</ul>
<h3>Input</h3>
<ul>
<li>Line 1: Q (1 ¡Ü Q ¡Ü 200000), the number of   operations</li>
<li>In the next Q lines, the first token of each line is a character   I, D, K or C meaning that the corresponding operation is   INSERT, DELETE, K-TH or COUNT, respectively, following   by a whitespace and an integer which is the parameter for that   operation.</li>
</ul>
<p>If the parameter is a value x, it is guaranteed that 0 ¡Ü |x|   ¡Ü 10<sup>9</sup>. If the parameter is an index k, it is   guaranteed that 1 ¡Ü k ¡Ü 10<sup>9</sup>.</p>
<h3>Output</h3>
<p>For each query, print the corresponding result in a single   line. In particular, for the queries K-TH, if k is larger than the   number of elements in S, print the word 'invalid'.</p>
<h3>Example</h3>
<pre><strong>Input</strong>
8
I -1
I -1
I 2
C 0
K 2
D -1
K 1
K 2

<strong>Output</strong>
1
2
2
invalid
</pre>
<p> </p>