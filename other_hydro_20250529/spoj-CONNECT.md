<p>
Byteotian Ministry of Infrastructure has decided to create a computer program
that helps to find quickly the lengths of routes between arbitrary towns. It
would be small wonder if the inhabitants of Byteotia always wanted to find the
shortest route. However, it happens that they want to know the <i>k</i>-th
shortest route. Moreover, cycles in routes are possible, i.e. routes that have
recurring towns.
</p>
<p>
For example, if there are 4 routes between two towns and their lengths are 2, 4, 4 and 5, then the length of the shortest connection is 2, the second shortest is 4, the third is 4, and the fourth is 5.
</p>

<h3>Task</h3>
<p>
Write a program that for each test case:
</p><ul>
  <li>Reads a description of Byteotian road network and
    queries concerning lengths of journey routes.
  </li><li>Computes and writes answers to the queries read.</li>
</ul>
<p></p>

<h3>Input</h3>
<p>
One integer in the first line, stating the number of test cases, followed by a blank line. There will be not more than 15 tests. 
</p>

<p>
For each test case, at the first line, there are two positive integers <i>n</i> and <i>m</i>, separated by a single space, 1 &lt;= <i>n</i> &lt;= 100, 0 &lt;= <i>m</i>
&lt;= <i>n</i><sup>2</sup>-<i>n</i>. They are the number of towns in Byteotia and the number of roads connecting the towns, respectively. The towns are numbered from 1 to <i>n</i>.
</p>
<p>
In each of <i>m</i> successive lines there are three integers separated by single spaces: <i>a</i>, <i>b</i> and <i>l</i>, <i>a</i> &lt;&gt; <i>b</i>, 1
&lt;= <i>l</i> &lt;= 500. Each triple describes one one-way road of length <i>l</i>
enabling to move from the town <i>a</i> to <i>b</i>. For each two towns there
exist at most one road that enables to move in the given direction.
</p>
<p>
In the following line there is one integer <i>q</i>, 1 &lt;= <i>q</i> &lt;= 10000, denoting the number of queries. In the successive <i>q</i> lines there are queries written, one per line. Each query has a form of three integers separated by single spaces: <i>c</i>, <i>d</i> and <i>k</i>, 1 &lt;= <i>k</i> &lt;= 100. Such a query refers to the length of the <i>k</i>-th shortest route from the town <i>c</i> to the town <i>d</i>.
</p>
<p>
The test cases will be separated by a single blank line. 
</p>

<h3>Output</h3>
<p>
For each test case, your program should write the answers to the queries read, one answer per line. In the i-th line the answer to the i-th query should be written: one integer equal to the length of the route being sought or -1, when such a route does not exist.
</p>
<p>
Each test case should be separated by a single blank line. 
</p>

<h3>Example</h3>

<pre><b>Input:</b>
1

5 5
1 2 3
2 3 2
3 2 1
1 3 10
1 4 1
8
1 3 1
1 3 2
1 3 3
1 4 2
2 5 1
2 2 1
2 2 2
1 1 2

<b>Output:</b>
5
8
10
-1
-1
3
6
-1
</pre>