<p>
You are given a sequence A[1], A[2], ..., A[N] . ( |A[i]| &lt;= 10000 , 1 &lt;= N &lt;= 10000 ). A query is
defined as follows:
Query(x1,y1,x2,y2) = Max { A[i]+A[i+1]+...+A[j] ; x1 &lt;= i &lt;= y1 , x2 &lt;= j &lt;= y2 and x1 &lt;= x2 , y1 &lt;= y2 }.
Given M queries (1 &lt;= M &lt;= 10000), your program must output the results of these queries.


</p><h3>Input</h3>
<p>
The first line of the input consist of the number of tests cases &lt;= 5.
Each case consist of the integer N and the sequence A. Then the integer M. 
M lines follow, contains 4 numbers x1, y1, x2 y2.


</p><h3>Output</h3>
<p>
Your program should output the results of the M queries for each test case, one query per line.


</p><h3>Example</h3>

<pre><b>Input:</b>
2
6 3 -2 1 -4 5 2
2
1 1 2 3
1 3 2 5
1 1
1
1 1 1 1

<b>Output:</b>
2
3
1


</pre>