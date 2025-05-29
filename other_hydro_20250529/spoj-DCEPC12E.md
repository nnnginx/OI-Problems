<p>Its holiday time after exams and Kappi and Pushap are enjoying to its fullest. But the sadist Sid, their&nbsp;</p>
<p>teacher, can¡¯t see them enjoy. Sad isn¡¯t it? To ruin their fun, he gave them a programming problem to be&nbsp;</p>
<p>solved within next 5 hours. He gives them 2 square matrices of equal dimension, Matrix A and a Matrix&nbsp;</p>
<p>B and asks multiple queries on these matrices. The queries will be to change a particular element of one&nbsp;</p>
<p>of the matrix and output the sum of elements of product of their matrix. Sid asks a lot of such queries.&nbsp;</p>
<p>Kappi and Pushap don¡¯t want the end of fun and so they ask you to solve this problem on behalf of&nbsp;</p>
<p>them.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line consists of N, the dimension of matrix.</p>
<p>Each of the next N lines contains N space separated integers. This is matrix A.</p>
<p>Each of the next N lines contains N space separated integers. This is matrix B.</p>
<p>Next line contains Q, the number of queries asked by Sid.</p>
<p>Each of the next Q lines consists of queries of the form ¡°A i j K¡± or ¡°B i j K¡± (quotes for clarity), meaning&nbsp;</p>
<p>change the element in ith row and jth column of matrix A or B to value K.</p>
<h3>Output</h3>
<p>Output exactly Q lines corresponding to Q queries, each containing the sum of the elements of the&nbsp;</p>
<p>matrix A*B.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2

1 2

3 4

4 3

2 1

3

A 1 1 2

B 0 1 3

A 0 0 10

<strong>Output:</strong>
40

40

103
</pre>
<pre><strong>Constraints:</strong>

1&lt;=N&lt;=100

1&lt;=Q&lt;=100000

0&lt;=i,j&lt;N

-10^6 &lt;= A[i][j], B[i][j] &lt;= 10^6<span style="white-space: normal;">
</span></pre>