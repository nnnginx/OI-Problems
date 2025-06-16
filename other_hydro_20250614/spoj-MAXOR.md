<p>
You are given a sequence A[1], A[2], ..., A[N]. (0 ¡Ü&nbsp;A[i] &lt;&nbsp;2<sup>31</sup>, 1 ¡Ü N ¡Ü 12000).</p>

<p>A query is defined as follows:
</p><ul>
  <li>Query(x,y) = Max { a[i] xor a[i+1] xor ... xor a[j] ; l ¡Ü i ¡Ü j ¡Ü r }.</li>
  <li>l = min (&nbsp;((x+lastans) mod N)+1 ,&nbsp;((y+lastans) mod N)+1&nbsp;).</li>
  <li>r = max (&nbsp;((x+lastans) mod N)+1 ,&nbsp;((y+lastans) mod N)+1&nbsp;).</li>
  <li>lastans[1] = 0 , lastans[i] = Query[i-1].</li>
</ul>

<p>
Given M queries, your program must output the results of these queries. (0 ¡Ü&nbsp;M ¡Ü 6000).</p>

<p><strong>IMPORTANT : PROBLEM ENHANCED. ( I'M SO SORRY.. )</strong></p>

<h3>Input</h3>
<ul>
<li>The first line of the input file contains 2 numbers : N M.</li>
<li>In the second line, N numbers follow.</li>
<li>M lines follow, where line i contains 2 numbers xi and yi.</li>
</ul>

<h3>Output</h3>
<p>Your program should output the results of the M queries, one query per line.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3 3
1 4 3
0 1
0 1
4 3

<strong>Output:</strong>
5
7
7</pre>