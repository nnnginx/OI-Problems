<p>
	The Stirling number of the second kind S(n, m) stands for the number of ways to 
	partition a set of n things into m nonempty subsets. For example, there are 
	seven ways to split a four-element set into two parts: {1, 2, 3} u {4}, {1, 2, 
	4} u {3}, {1, 3, 4} u {2}, {2, 3, 4} u {1}, {1, 2} u {3, 4}, {1, 3} u {2, 4}, 
	{1, 4} u {2, 3}.
</p>
<p>
	There is a recurrence which allows you to compute S(n, m) for all m and n.<br>
	S(0, 0) = 1,<br>
	S(n, 0) = 0, for n &gt; 0,<br>
	S(0, m) = 0, for m &gt; 0,<br>
	S(n, m) = m*S(n-1, m) + S(n-1, m-1), for n, m &gt; 0.
</p>
<p>
	Your task is much "easier". Given integers n and m satisfying 1 &lt;= m &lt;= 
	n, compute the parity of S(n, m), i.e. S(n, m) mod 2.
</p>
<p>
	For instance, S(4, 2) mod 2 = 1.
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads two positive integers n and m,
		</li><li>
		computes S(n, m) mod 2,
		</li><li>
			writes the result.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The first line of the input contains exactly one positive integer d equal to 
	the number of data sets, 1 &lt;= d &lt;= 200. The data sets follow.
</p>
<p>
	Line i + 1 contains the i-th data set - exactly two integers n<sub>i</sub> and 
	m<sub>i</sub> separated by a single space, 1 &lt; = m<sub>i</sub> &lt; = n<sub>i</sub>
	&lt;= 10<sup>9</sup>.
</p>
<h3>Output</h3>
<p>
	The output should consist of exactly d lines, one line for each data set. Line 
	i, 1 &lt;= i &lt; = d, should contain 0 or 1, the value of S(n<sub>i</sub>, m<sub>i</sub>) 
	mod 2.
</p>
<h3>Example</h3>
<pre><b>Sample input:</b>
1
4 2

<b>Sample output:</b>
1
</pre>