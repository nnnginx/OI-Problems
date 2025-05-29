<p>Given N non negative numbers, the task is to answer M queries.</p>
<p>Each query is as follows:&nbsp;</p>
<p>Given u,v you need to find the pairwise product sum (u and v are zero indexed)</p>
<p>a<sub>u</sub>a<sub>u</sub> + a<sub>u+1</sub>a<sub>u+1</sub>&nbsp;+ a<sub>u+1</sub>a<sub>u</sub>&nbsp;+ a<sub>u+2</sub>a<sub>u+2</sub>&nbsp;+ a<sub>u+2</sub>a<sub>u+1</sub>&nbsp;+ a<sub>u+2</sub>a<sub>u</sub>&nbsp;+ ... + a<sub>v</sub>a<sub>v</sub>&nbsp;+ a<sub>v</sub>a<sub>v-1</sub>&nbsp;+ ... + a<sub>v</sub>a<sub>u</sub></p>

<h3>Input</h3>
<pre>N
a<sub>0</sub> a<sub>1</sub> ... a<sub>N-1</sub>
M
u<sub>1</sub> v<sub>1</sub>
u<sub>2</sub> v<sub>2</sub>
...
u<sub>M</sub> v<sub>M</sub></pre>

<h3>Output</h3>

<p>Print the answer for each query in a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
2 0 1 3 3
3
0 2
1 2
3 4

<strong>Output:</strong>
7
1
27</pre>

<h3>Constraints</h3>
<p>
0 &lt;= u &lt;= v &lt; N <br>
N &lt;= 100000<br>
M &lt;= 100000<br>
0 &lt;= a<sub>i</sub> &lt;= 1000000

</p>