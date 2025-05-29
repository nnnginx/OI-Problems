<p>
Assume that you are a manager and there are m types of worker (numbered from 1 to m) and n types of task (numbered from 1 to n). There are a(i) workers of type #i and b(j) postitions for task #j. C(i, j) is the cost of hiring a worker of type #i to do the task of type #j. Your job is to minimize the cost of hiring workers to fill all the positions given that the total number of workers is equal to the total number of positions.
</p><h3>Input</h3>
<p>
The first line of input contains the number of test cases nTest (1&lt;= nTest &lt;= 10). 
 Each test case contains:
</p><ul>
<li>The first line contains the number of worker types - m and number of task types - n. 
</li><li>The second line contains m positive integers: a(1), a(2), ..., a(m).
</li><li>The third line contains n positive integers: b(1), b(2), ..., b(n).
</li><li>Each of the next m lines contains n integers describing matrix C(i, j).
</li></ul>
<p>Notes: </p><p>
1 &lt;= m, n &lt;= 200; </p><p>
1 &lt;= a(i), b(i) &lt;= 30000; </p><p>
1 &lt;= C(i, j) &lt;= 10000. </p><p>
Sum of a(i) equals to sum of b(j).
</p><h3>Output</h3>
<p>
For each test case write the minimum cost in a separate line (it will fit in a signed 32-bit integer).

</p><h3>Example</h3>

<pre><b>Input:</b>
2
3 4
3 6 7
2 5 1 8
1 2 3 4
8 7 6 5
9 12 10 11
4 4
1 3 5 7
2 4 2 8
1 4 7 3
4 7 5 3
5 7 8 3
5 3 6 8

<b>Output:</b>
110
54
</pre>