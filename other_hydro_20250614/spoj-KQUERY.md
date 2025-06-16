<!--  Note: this problem already appears in the main problemset as: http://www.spoj.com/problems/RACETIME/  -->
<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/KQUERY/en/">English</a></td>
<td width="50%"><a href="/problems/KQUERY/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Given a sequence of n numbers a<sub>1</sub>,   a<sub>2</sub>, ..., a<sub>n</sub> and a number of k-  queries. A k-query is a triple (i, j, k) (1 ¡Ü i ¡Ü j ¡Ü n). For   each k-query (i, j, k), you have to return the number of   elements greater than k in the subsequence a<sub>i</sub>,   a<sub>i+1</sub>, ..., a<sub>j</sub>.</p>
<h3>Input</h3>
<ul>
<li>Line 1: n (1 ¡Ü n ¡Ü 30000).</li>
<li>Line 2: n numbers a<sub>1</sub>, a<sub>2</sub>, ...,   a<sub>n</sub> (1 ¡Ü a<sub>i</sub> ¡Ü   10<sup>9</sup>).</li>
<li>Line 3: q (1 ¡Ü q ¡Ü 200000), the number of k-  queries.</li>
<li>In the next q lines, each line contains 3 numbers i, j, k   representing a k-query (1 ¡Ü i ¡Ü j ¡Ü n, 1 ¡Ü k ¡Ü   10<sup>9</sup>).</li>
</ul>
<h3>Output</h3>
<ul>
<li>For each k-query (i, j, k), print the number of elements   greater than k in the subsequence a<sub>i</sub>,   a<sub>i+1</sub>, ..., a<sub>j</sub> in a single line.
<p>&nbsp;</p>
</li>
</ul>
<h3>Example</h3>
<pre><strong>Input</strong>
5
5 1 2 3 4
3
2 4 1
4 4 4
1 5 2 

<strong>Output</strong>
2
0
3 
</pre>
<p> </p>