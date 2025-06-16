<p>
	A <i>partition</i> of positive integer m into n components is any sequence a<sub>1</sub>,...,a<sub>n</sub>
	of positive integers such that a<sub>1</sub>+...+a<sub>n</sub>=m and a<sub>1</sub>&lt;=a<sub>2</sub>&lt;=...&lt;=a<sub>n</sub>. 
	Your task is to determine the partition, which occupies the k-th position in 
	the lexicographic order of all partitions of m into n components.
</p>
<p>
	The lexicographic order is defined as follows: sequence a<sub>1</sub>,...,a<sub>n</sub>
	comes before b<sub>1</sub>,...,b<sub>n</sub> iff there exists such an integer 
	i,1&lt;=i&lt;=n, that a<sub>j</sub>=b<sub>j</sub>
	for all j, 1&lt;= j&lt; i, and a<sub>i</sub>&lt; b<sub>i</sub>.
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case the input consists of three lines, containing the positive 
	integers m, n and k respectively (1&lt;=n&lt;= 10, 1&lt;= m&lt;=220, k is not 
	larger than the number of partitions of m into n components).
</p>
<h3>Output</h3>
<p>
	For each test case output the ordered elements of the sought partition, 
	separated by spaces.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
9
4
3

<b><tt>Sample output:</tt></b>
1 1 3 4
</pre>