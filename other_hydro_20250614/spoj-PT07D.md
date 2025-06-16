<p>
Given two integer <i>n</i>, <i>p</i>. 4 kinds of query is needed to solve:</p>
<p>
1. Counting the number of labeled unrooted trees with <i>n</i> nodes<br>
2. Counting the number of labeled rooted trees with <i>n</i> nodes<br>
3. Counting the number of unlabeled rooted trees with <i>n</i> nodes<br>
4. Counting the number of unlabeled unrooted trees with <i>n</i> nodes<br>
Calculate the answer modulo <i>p</i>.

</p><h3>Input</h3>
<p>
Each line contains three integers <i>k</i>, <i>n</i>, <i>p</i>. <i>k</i> denotes which kind of query this
case is.<br>
For Kind 1 or Kind 2 query, 1 &lt;= <i>n</i> &lt;= 10<sup>9</sup>.<br>
For Kind 3 or Kind 4 query, 1 &lt;= <i>n</i> &lt;= 10<sup>3</sup> and <i>n</i> &lt;= <i>p</i>.<br>
For all queries, 2 &lt;= <i>p</i> &lt;= 10<sup>4</sup> and <i>p</i> is a prime.

</p><h3>Output</h3>
<p>
For each query, output a line which contains only one integer.

</p><h3>Example</h3>

<pre><b>Input:</b>
1 2 2
2 2 3
3 2 5
4 2 3

<b>Output:</b>
1
2
1
1
</pre>