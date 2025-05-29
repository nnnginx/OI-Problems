<p>You are given N integers, A[1] to A[N]. You have to assign weights to  these integers such that their weighted sum is maximized. The weights  should satisfy the following conditions :</p>
<ol>
<li> Each weight should be an positive integer. </li>
<li> W[1] = 1 </li>
<li> W[i] should be in the range [2, W[i-1] + 1] for i &gt; 1 </li>
</ol>
<p>Weighted sum is defined as S = A[1] * W[1] + A[2] * W[2] + ... + A[N] * W[N]</p>
<h3>Input</h3>
<p>There are multiple test cases. <br> First line contains the number of test cases <br> Each test case consists of a single line containing N. <br> This is followed by N lines, each containing A[i]</p>
<h3>Output</h3>
<p>For each test case, output one line - the maximum weighted sum.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1 <br>4 <br>1 <br>2 <br>3 <br>-4<br><strong>Output:</strong>
6<br><strong>Explanation<br></strong>The weights are 1,2,3,2<br><br></pre>
<h3>Constraints</h3>
<p>N &lt;= 10^6 <br> | A[i] | &lt;= 10^6 <br> Total number of test cases is around 10.</p>