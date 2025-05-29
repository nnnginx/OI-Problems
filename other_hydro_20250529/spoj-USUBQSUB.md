<p>Updating and querying 1 dimensional arrays is a popular question. How about updating and quering sub-matrices of a matrix?</p>
<p>A sub-matrix will be depicted as (a, b), (c, d). This implies that it will include all the cells (x, y) such that a&lt;=x&lt;=c and b&lt;=y&lt;=d.</p>
<p>The matrix is indexed from [1..N][1..N], where N is the size.</p>
<p>&nbsp;</p>
<p>You are given a matrix of size NxN, with each element initially set to 0. There are M queries and each query can be of one of the two types:</p>
<p>1 x1 y1 x2 y2: This query asks you to return the sum of all the elements in the sub-matrix (x1, y1), (x2, y2).</p>
<p>2 x1 y1 x2 y2 K: This query asks you to add K to each element in the sub-matrix (x1, y1), (x2, y2).</p>
<h3>Input</h3>
<p>The first line of input contains N, M.</p>
<p>The next M lines contain queries in the same forms as stated above.</p>
<p>You may assume that x1&lt;=x2 and y1&lt;=y2 for all queries.</p>
<p>Also N&lt;=1000 and M&lt;=10<sup>5</sup>. K&lt;=10<sup>9</sup></p>
<h3>Output</h3>
<p>The answer to all the queries wherein you need to return the sum of elements in the sub-matrix, i.e., all the queries of type 1.</p>
<p>&nbsp;</p>
<h3>Sample Test Case</h3>
<pre><strong>Input:</strong>
5 5<br>2 2 2 4 4 4<br>1 1 1 3 3<br>2 5 5 5 5 3<br>1 1 1 1 2<br>1 2 2 5 3<br><strong>Output:</strong>
16<br>0<br>24<br><br><strong>Note: </strong>Please be careful with certain languages as the output may exceed the range of the data type used to store it.<br>         Please use 64-bit integers to store the results. For example, long long in C/C++.</pre>