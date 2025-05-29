<p>There are N numbers a[0],a[1]..a[N - 1]. 
Initally all are 0. You have to perform two types of operations :<br><br>
1) Increase the numbers between indices A and B (inclusive) by 1. 
This is represented by the command "0 A B"<br>
2) Answer how many numbers between indices A and B (inclusive) are divisible by 3. 
This is represented by the command "1 A B".<br></p>

<h3>Input</h3>
<p>The first line contains two integers, N and Q. 
Each of the next Q lines are either of the form "0 A B" or "1 A B" as mentioned above.</p>

<h3>Output</h3>
<p>Output 1 line for each of the queries of the form "1 A B" containing the required answer for the corresponding query.</p>

<h3>Sample</h3>
<pre><strong>Sample Input :</strong>
4 7
1 0 3
0 1 2
0 1 3
1 0 0
0 0 3
1 3 3
1 0 3

<strong>Sample Output :</strong>
4
1
0
2</pre>

<h3>Constraints</h3>
<p>1 &lt;= N &lt;= 100000<br>
1 &lt;= Q &lt;= 100000<br>
0 &lt;= A &lt;= B &lt;= N - 1</p>