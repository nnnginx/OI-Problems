<p>You are given a sequence A of N(N &lt;= 100,000) positive integers. There sum will be less than 10<sup>18</sup>. On this sequence you have to apply M (M &lt;= 100,000) operations:</p>
<p>(A) For given x,y, for each elements between&nbsp;the x-th and the y-th ones (inclusively, counting from 1), modify it to its positive square root (rounded down to the nearest integer).</p>
<p>(B) For given x,y, query the sum of all the elements between the x-th and the y-th ones (inclusively, counting from 1) in the sequence.</p>
<h3>Input</h3>
<p>Multiple test cases, please proceed them one by one. Input terminates by EOF.</p>
<p>For each test case:</p>
<p>The first line contains an integer N. The following line contains N integers, representing the sequence A<sub>1</sub>..A<sub>N</sub>. <br> The third line contains an integer M. The next M lines contain the operations in the form "i x y".i=0 denotes the modify operation, i=1 denotes the query operation.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>Output the case number (counting from 1) in the first line of output. Then for each query, print an integer as the problem required.</p>
<p>Print an blank line after each test case.</p>
<p>See the sample output for more details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
1 2 3 4 5
5
1 2 4
0 2 4
1 2 4
0 4 5
1 1 5
4
10 10 10 10
3
1 1 4
0 2 3
1 1 4

<strong>Output:</strong>
Case #1:
9
4
6

Case #2:
40
26

</pre>