<p>You are given a sequence of <strong>n</strong> integers
<strong>a<sub>1</sub> , a<sub>2</sub> , ... , a<sub>n</sub></strong>
in non-decreasing order. In addition to that, you are given several
queries
consisting of indices <strong>i</strong> and <strong>j</strong> (<i>1
¡Ü i ¡Ü j ¡Ü n</i>). For each query, determine the
most
frequent value among the integers <strong>a<sub>i</sub> , ... , a<sub>j</sub></strong>.
</p>
<h4>Input Specification</h4>
<p>
The input consists of several test cases.
Each test case starts with a line containing two integers <strong>n</strong>
and <strong>q</strong> (<i>1 ¡Ü n, q ¡Ü 100000</i>).
The next line contains <strong>n</strong> integers
<strong>a<sub>1</sub> , ... , a<sub>n</sub></strong>
(<i>-100000 ¡Ü a<sub>i</sub> ¡Ü 100000</i>, for each <i>i ¡Ê {1, ..., n}</i>)
separated by spaces.
You can assume that for each <i>i ¡Ê {1, ..., n-1}: a<sub>i</sub> ¡Ü a<sub>i+1</sub></i>.
The following <strong>q</strong> lines contain one query each,
consisting of two integers <strong>i</strong> and <strong>j</strong>
(<i>1 ¡Ü i ¡Ü j ¡Ü n</i>), which indicate the boundary indices for the
query.
</p>
<p>
The last test case is followed by a line containing a single <i>0</i>.
</p>
<h4>Output Specification</h4>
<p>
For each query, print one line with one integer:
The number of occurrences of the most frequent value within
the given range.
</p>
<h4>Sample Input</h4>
<pre>10 3
-1 -1 1 1 1 1 3 10 10 10
2 3
1 10
5 10
0
</pre>
<h4>Sample Output</h4>
<pre>1
4
3
</pre>
<hr>
<i>A naive algorithm may not run in time!</i>