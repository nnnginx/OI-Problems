<p>Let S be the binary representation of an Integer. We define two functions a(i) and b(i) such that<br> a(i) = Number of occurrences of '1' at odd positions of S.<br> b(i) = Number of occurrences of '1' at even positions of S.<br> For example: for integer 19, S=10011.<br> so, a(19)=2 and b(19)=1</p>
<h3>Input</h3>
<p>First line contains an integer T. T=Number of test cases. Then T lines follow<br> On each line, you will be given three integers M,N,K.</p>
<h3>Output</h3>
<p>For each test case output a single integer R.<br> Where, R is the number of integers 'i' between M and N(both inclusive) such that absolute difference of a(i) and b(i) is equal to K.<br>Answer of each each test case should be on separate line</p>
<h3>Constraints</h3>
<p>T&lt;=50<br> 1&lt;=M&lt;N&lt;=10^19 <br>1&lt;=N-M&lt;=10^6 <br>0&lt;=K&lt;=50</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
1 10 2

<strong>Output:</strong>
2
</pre>