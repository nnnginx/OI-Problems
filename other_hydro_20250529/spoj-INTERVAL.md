<p>
	You are given n closed integer intervals [a<sub>i</sub>, b<sub>i</sub>] and n 
	integers c<sub>1</sub>, ..., c<sub>n</sub>.
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
			reads the number of intervals, their endpoints and integers c<sub>1</sub>, ..., 
			c<sub>n</sub>
		from the standard input,
		</li><li>
			computes the minimal size of a set Z of integers which has at least c<sub>i</sub>
			common elements with interval [a<sub>i</sub>, b<sub>i</sub>], for each i = 
		1, 2, ..., n,
		</li><li>
			writes the answer to the standard output.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case the first line of the input contains an integer n (1 &lt;= n 
	&lt;= 50000) - the number of intervals. The following n lines describe the 
	intervals. Line (i+1) of the input contains three integers a<sub>i</sub>, 
	b<sub>i</sub> and c<sub>i</sub> separated by single spaces and such that 0 &lt; 
		= a<sub>i</sub> &lt; = b<sub>i</sub> &lt;= 50000 and 1 &lt; = c<sub>i</sub> &lt; 
		= b<sub>i</sub> -a<sub>i</sub> +1.
</p>
<h3>Output</h3>
<p>
	For each test case the output contains exactly one integer equal to the minimal 
	size of set Z sharing at least c<sub>i</sub> elements with interval [a<sub>i</sub>, 
	b<sub>i</sub>], for each i= 1, 2, ..., n.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
5
3 7 3
8 10 3
6 8 1
1 3 1
10 11 1

<b><tt>Sample output:</tt></b>
6
</pre>
<b>Warning: enormous Input/Output data, be careful with certain languages</b>