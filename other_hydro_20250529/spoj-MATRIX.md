<p>You are given a matrix A of M rows and N columns, consisting of numbers 0 and 1. For a rectangle in A (sides &gt;= 1), X1 is the number of ones on its sides, X0 is the number of zeros on its sides, and its <i>value</i> is defined as X1 ¨C X0. Let us consider W, the maximum value taken over submatrices of A, and S, the number of submatrices with value W. Your task is to find W and S.

</p><h3>Input</h3>
<p>The first line of input contains the number of testcases t (t &lt;= 15).
The first line of each testcase contains the numbers M, N (1 &lt;= M, N &lt;= 200) Then M lines follow. In each line, there are N numbers 0 or 1. 

</p><h3>Output</h3>
<p>For each testcase, you should output a single line with numbers W and S.
</p><h3>Example</h3>

<pre><b>Input:</b>
1
5 6
1 1 1 1 1 1
1 0 0 0 0 1
1 0 0 0 0 1
1 0 0 0 0 1
1 1 1 1 1 1

<b>Output:</b>
18 1
</pre>