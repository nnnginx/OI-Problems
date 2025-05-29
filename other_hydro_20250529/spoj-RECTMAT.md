<p>In a matrix with n rows and m columns, (i,j) is the cell in i-th row and  j-th column(0&lt;=i&lt;n,0&lt;=j&lt;m). A rectangle (r0,r1,c0,c1) in a  matrix is the set of cells (i,j) where r0 &lt;= i &lt; r1 and c0 &lt;= j  &lt; c1. (0&lt;=r0 &lt; r1 &lt;= n, 0 &lt;= c0 &lt;c1 &lt;= m). Two  rectangles are called independent if the intersection of their cell set  is empty.<br> Given n,m,k, find the number of ways to choose k  independent rectangles from a nxm matrix. The order of these k  rectangles doesn't matter, see sample for further clarification.</p>
<h3>Input</h3>
<p><br> One line contains three integers n,m,k(1&lt;=n,m&lt;=1000, 1&lt;=k&lt;=6).</p>
<h3>Output</h3>
<p>For each test case, output the number of ways, modulo 10^9+7.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2 2 4<br>10 10 1<br><strong>Output:</strong><br>1<br>3025<br><strong>Explanation<br></strong>First case: You have to find the number of ways of choosing 4  independent rectangles from a 2x2 matrix.<br>The only way to do this is to  choose each cell as a separate rectangle.<br><br></pre>
<h3>Constraints</h3>
<p>(1&lt;=n,m&lt;=1000, 1&lt;=k&lt;=6).<br> Total number of test cases is around 150. Not all the test cases are included.</p>