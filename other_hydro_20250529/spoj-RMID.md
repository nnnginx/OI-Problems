<p>
You will be given some integers in non decreasing order and each time the median is queried you have to report and remove it. Take the smaller element as median in case of even elements.
</p>

<h3>Input</h3>
<p>
The input contains many test cases. Read until End Of File.
</p>
<p>
Each test case contains n (n ¡Ü 100000) positive integers in non-decreasing order,&nbsp;along with m queries indicated by -1, all on separate lines. (See the example.)
</p>
<p>
For a query, print the current median on a single line and remove it from the list.&nbsp;
</p>
<p>
Each test case ends with 0 on a single line, and two test cases will be separated by an empty line. All integers are guaranteed to fit in a signed 32-bit container.&nbsp;A query can only occur if the list is non-empty.&nbsp;</p>

<h3>Output</h3>
<p>
For each test case output m lines containing the answers to the corresponding queries.&nbsp;Print an empty line after each test case.&nbsp;</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1
2
3
4
-1
-1
5
6
7
-1
0

2
3
-1
0

<b>Output:</b>
2
3
5

2</pre>