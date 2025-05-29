<p>
Let A[0...n - 1] be an array of n distinct positive integers. 
If i &lt; j and A[i] &gt; A[j] then the pair (i, j) is called an inversion of A. 
Given n and an array A your task is to find the number of inversions of A.
</p>

<h3>Input</h3>
<p>The first line contains t, the number of testcases followed by a blank space. 
Each of the t tests start with a number n (n &lt;= 200000). 
Then n + 1 lines follow. In the ith line a number A[i - 1] is given (A[i - 1] &lt;= 10^7). 
The (n + 1)th line is a blank space.</p>

<h3>Output</h3>
<p>For every test output one line giving the number of inversions of A.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2

3
3
1
2

5
2
3
8
6
1


<strong>Output:</strong>
2
5</pre>