<p>
	You are given:
</p>
<div align="left">
	<ul>
		<li>
		a positive integer n,
		</li><li>
		an integer k, 1&lt;=k&lt;=n,
		</li><li>
			an increasing sequence of k integers 0 &lt; s<sub>1</sub> &lt; s<sub>2</sub> &lt; 
			... &lt; s<sub>k</sub> &lt;= 2n.</li>
	</ul>
</div>
<p>
	What is the number of proper bracket expressions of length 2n with opening 
	brackets appearing in positions s<sub>1</sub>, s<sub>2</sub>,...,s<sub>k</sub>?
</p>
<h3>Illustration</h3>
<p>Several proper bracket expressions:</p>
<pre><tt>[[]][[[]][]] 
[[[][]]][][[]]</tt></pre><p>An improper bracket expression:</p>
<pre><tt>[[[][]]][]][[]]</tt></pre><p>
	There is exactly one proper expression of length 8 with opening brackets in 
	positions 2, 5 and 7.
</p>
<h3>Task</h3>
<p>
	Write a program which for each data set from a sequence of several data sets:
</p>
<div align="left">
	<ul>
		<li>
		reads integers n, k and an increasing sequence of k integers from input,
		</li><li>
			computes the number of proper bracket expressions of length 2n with opening 
			brackets appearing at positions s<sub>1</sub>,s<sub>2</sub>,...,s<sub>k</sub>,
		</li><li>
			writes the result to output.</li>
	</ul>
</div>
<h3>
	Input
</h3>
<p>
	The first line of the input file contains one integer d, 1 &lt;= d &lt;= 10, 
	which is the number of data sets. The data sets follow. Each data set occupies 
	two lines of the input file. The first line contains two integers n and k 
	separated by single space, 1 &lt;= n &lt;= 19, 1 &lt;= k &lt;= n. The second 
	line contains an increasing sequence of k integers from the interval [1;2n] 
	separated by single spaces.
</p>
<h3>
	Output
</h3>
<p>
The i-th line of output should contain one integer - the number of proper 
bracket expressions of length 2n with opening brackets appearing at positions s<sub>1</sub>, 
s<sub>2</sub>,...,s<sub>k</sub>.</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
5 
1 1 
1 
1 1 
2 
2 1 
1 
3 1 
2 
4 2 
5 7 

<b><tt>Sample output:</tt></b>
1 
0 
2 
3 
2 
</pre>