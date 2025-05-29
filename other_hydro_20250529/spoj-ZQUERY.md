<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/ZQUERY/en">English</a></td>
<td width="50%"><a href="/problems/ZQUERY/vn">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Given an array having <strong>N</strong> elements, each element is either <strong>-1</strong> or <strong>1</strong>.</p>
<p>You have <strong>M</strong> queries, each query has two numbers <strong>L</strong> and <strong>R</strong>, you have to answer the length of the longest subarray in range <strong>L</strong> to <strong>R</strong> (inclusive) that its sum is equal to <strong>0</strong>.</p>
<h3>Input</h3>
<p>The first line contains two numbers <strong>N</strong> and <strong>M</strong> (<strong>1</strong> &lt;= <strong>N</strong>, <strong>M</strong> &lt;= <strong>50000</strong>) - the number of elements and the number of queries.</p>
<p>The second line contains <strong>N</strong> numbers - the elements of the array, each element is either <strong>-1</strong> or <strong>1</strong>.</p>
<p>In the next <strong>M</strong> lines, each line contains two numbers <strong>L</strong> and <strong>R</strong> (<strong>1</strong> &lt;= <strong>L</strong> &lt;= <strong>R</strong> &lt;= <strong>N</strong>).</p>
<h3>Output</h3>
<p>For each query, print the length of the longest subarray that satisfies the query in one line. If there isn't any such subarray, print <strong>0</strong>.</p>
<h3>Note</h3>
<p>Subarray in an array is like substring in a string, i.e. subarray should contain contiguous elements.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 4
1 1 1 -1 -1 -1
1 3
1 4
1 5
1 6</pre>
<pre><strong>Output:</strong>
0
2
4
6</pre>
<p></p>