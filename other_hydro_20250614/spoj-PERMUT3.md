<p>Given a permutation of <b>n</b> elements (1, 2, ..., n): A = (a<sub>1</sub>, a<sub>2</sub>, ..., a<sub>n</sub>). We define a sequence P(A)=(p<sub>1</sub>, p<sub>2</sub>, бн, p<sub>n-1</sub>) where p<sub>i</sub> = 0 if a<sub>i</sub> &gt; a<sub>i+1</sub> and p<sub>i</sub> = 1 if a<sub>i</sub> &lt; a<sub>i+1</sub>. Given a permutation B, find the number of all permutations C where P(C)=P(B) including the permutation B itself.</p>
<p><b>The length of your solution should not be more than 0.5kB.</b></p>
<h3>Input</h3>
<p>Multiple test cases. For each test case:</p>
<p>The first line contains an integer <b>n</b>(1&lt;= <b>n</b> &lt;=100).The second line contains <b>n</b> integers representing the permutation, all of which are separated by single spaces.</p>
<p>Input terminates by a single zero.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>The output contains a single line with a single integer - the number of the permutations having the same value for P(A) when given the permutation A.</p>
<h3>Example</h3>
<pre><b>Input</b>:
2
1 2
4
1 3 2 4
0

<b>Output:</b>
1
5

</pre>