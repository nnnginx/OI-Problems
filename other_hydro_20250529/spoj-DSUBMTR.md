<p>Consider an matrix of capital letters. By selecting consecutive columns and rows, we can define the sub-matrix as the elements on chosen columns and rows.
</p><p>Two sub-matrices should be regarded the same if and only if they have the same detentions and characters (which, of course, are capital letters) on corresponding position. It is your task to find the number of distinct sub-matrices of a given letter matrix.
</p><h3>Input</h3>

<p>The input contains a lot of test cases. The first line of input contains exactly one integer, indicating the number of test cases.
</p><p>For each of the test case, the first line contains two integers <b>N</b> and <b>M</b>, denoting the number of rows and columns of the given matrix. (1 &lt;= <b>N</b>, <b>M</b> &lt;= 128)
</p><p>The next <b>N</b> lines contain only capital letters, indicating the given matrix.

</p><h3>Output</h3>

<p>For each test case, output a single integer denoting the number of distinct sub-matrices.

</p><h3>Example</h3>
<pre><b>Input:</b>
2
2 2
AB
BA
3 3
ABA
BAA
AAA

<b>Output:</b>
Case #1: 7
Case #2: 22
</pre>