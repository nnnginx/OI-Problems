<p>You are given a sequence A[1], A[2], ..., A[N] . ( |A[i]| ¡Ü  15007 , 1 ¡Ü N ¡Ü 50000 ). A query is defined as follows:
<br>
Query(x,y) = Max { a[i]+a[i+1]+...+a[j] ; x ¡Ü i ¡Ü j ¡Ü y }. 
<br> 
Given M queries, your program must output the results of these queries.
</p><h3>Input</h3>
<ul>
<li>The first line of the input file contains the integer N.</li>
<li>In the second line, N numbers follow.</li>
<li>The third line contains the integer M.</li>
<li>M lines follow, where line i contains 2 numbers xi and yi.</li>
</ul>

<h3>Output</h3>
<p>Your program should output the results of the M queries, one query per line. </p>

<h3>Example</h3>

<pre><b>Input:</b>
3 
-1 2 3
1
1 2

<b>Output:</b>
2
</pre>