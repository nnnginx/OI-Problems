<p>
Given an integer sequence containing n elements (numbered from 1 to n), your task is to find the minimum value M so that we can find k + 1 integers 0 = p(0) &lt; p(1) &lt; p(2) &lt; ... &lt; p(k-1) &lt; p(k) = n, such that for any i from 0 to k - 1, the sum of elements from  postition p(i)+1 to postition p(i+1) is not greater than M.

</p><h3>Input</h3>
<p>

The first line of input contains the number of test cases nTest (1 &lt;= nTest &lt;= 10). </p><p>
Each test case contains: </p><p>
The first line contains n, k. (1 &lt;= k &lt;= n &lt;= 15000) </p><p>
Each of the next n lines contains an integer of the sequence with value range from -30000 to 30000.

</p><h3>Output</h3>
<p>
For each test case write the minimum number M in a separate line.
</p><h3>Example</h3>

<pre><b>Input:</b>
1
9 4
1
1
1
3
2
2
1
3
1

<b>Output:</b>
5
</pre>