<p>You are given a positive integer N. Let us consider set A of fractions x/y where 0 &lt;= x/y &lt;= 1, y &lt;= N and the maximum common divisor of x and y is 1. </p>
<p>
For example N = 5. Set A in increasing order consists of elements 0/1; 1/5; 1/4; 1/3; 2/5; 1/2; 3/5; 2/3; 3/4; 4/5; 1/1.</p>
<p>
Your task is to find the i-th smallest fraction in set A.</p>
<h3>Input</h3>
<p>The first line of input contains the number of testcases t (t &lt;= 15). The first line of each testcase contains numbers N and M (N &lt;= 5000, M &lt;= 10000). The next M lines contain one question each.
</p><h3>Output</h3>
<p>For each testcase, you should output M lines which are the answers to the M questions.
</p><h3>Example</h3>

<pre><b>Input:</b>
1
5 4
1
3
5
8

<b>Output:</b>
0/1
1/4
2/5
2/3
</pre>