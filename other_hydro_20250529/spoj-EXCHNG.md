<p>
	Given n integer registers r<sub>1</sub>, r<sub>2</sub>, ... , r<sub>n</sub> we 
	define a Compare-Exchange Instruction CE(a,b), where a, b are register indices 
	(1 &lt;= a &lt; b &lt;= n):
</p>
<pre>CE(a, b):: 
  if content(r<sub>a</sub>) &gt;  content(r<sub>b</sub>) then 
     exchange the contents of registers r<sub>a</sub> and r<sub>b</sub>; 
</pre>
<p>
	A Compare-Exchange program (shortly CE-program) is any finite sequence of 
	Compare-Exchange instructions. A CE-program is called a Minimum-Finding program 
	if after its execution the register r<sub>1</sub> always contains the smallest 
	value among all values in the registers. Such a program is called reliable if 
	it remains a Minimum-Finding program after removing any single Compare-Exchange 
	instruction. Given a CE-program P, what is the smallest number of instructions 
	that should be added at the end of program P in order to get a reliable 
	Minimum-Finding program?
</p>
<p>
	For instance, consider the following CE-program for 3 registers: CE(1, 2), 
	CE(2, 3), CE(1, 2). In order to make this program a reliable Minimum-Finding 
	program it is sufficient to add only two instructions: CE(1, 3) and CE(1, 2).</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads the description of a CE-program,
		</li><li>
		computes the smallest number of CE-instructions that should be added to make 
		this program a reliable Minimum-Finding program,
		</li><li>
			writes the result.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The first line of the input contains exactly one positive integer d equal to 
	the number of data sets, 1 &lt;= d &lt;= 10. The data sets follow.
</p>
<p>
	Each data set consists of exactly two consecutive lines. The first of those 
	lines contains exactly two integers n and m separated by a single space, 2 
	&lt;= n &lt;= 10000, 0 &lt;= m &lt;= 25000. Integer n is the number of 
	registers and integer m is the number of program instructions.
</p>
<p>
	The second of those lines contains exactly 2m integers separated by single 
	spaces - the program itself. Integers a<sub>j</sub>, b<sub>j</sub> on positions 
	2j-1 and 2j, 1 &lt;= j &lt; = m, 1 &lt; = a<sub>j</sub> &lt; b<sub>j</sub> &lt;= 
	n, are parameters of the j-th instruction in the program.</p>
<h3>Output</h3>
<p>
	The output should consist of exactly d lines, one line for each data set. Line 
	i, 1 &lt;= i &lt;= d, should contain only one integer - the smallest number of 
	instructions that should be added at the end of the i-th input program in order 
	to make this program a reliable Minimum-Finding program.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1 
3 3 
1 2 2 3 1 2

<b><tt>Sample output:</tt></b>
2 
</pre>