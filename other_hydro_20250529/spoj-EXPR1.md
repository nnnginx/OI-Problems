<p>
	We are given an integer k and an arithmetic expression E with the operations 
	'+', '-', and arguments from the set {0,1,...,9}. Is it possible to put some 
	parentheses in E to get a new expression E' whose value equals k? If the answer 
	is positive what is the minimum number of pairs of parentheses '(', ')' that 
	are necessary?
</p>
<h3>Illustration</h3>
<p>
	It is sufficient to put one pair of parentheses in the expression 5 - 4 + 5 to 
	get an expression with value -4, namely 5 - (4 + 5) = -4.
</p>
<h3>Task
</h3>
<p>
	Write a program that for each data set from a sequence of several data sets:
</p>
<div align="justify">
	<ul>
		<li>
		reads an expression E and an integer k from input,
		</li><li>
		verifies whether it is possible to put some parentheses in E to get a new 
		expression E' whose value equals k and computes the minimal number of pairs of 
		parentheses '(', ')' necessary, if the answer is positive,
		</li><li>
			writes the result to output.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The first line of the input file contains one positive integer d not larger 
	than 10. This is the number of data sets. The data sets follow. Each set of 
	data occupies two consecutive lines of the input file. The first line contains 
	two integers n and k, 2 &lt;= n &lt;= 40, -180 &lt;= k &lt;= 180. The even 
	integer n is the length of E. The second line contains the expression itself 
	written as a string of length n. The string contains operators '+' or '-' in 
	odd positions and numbers from the set {0,1,...,9} in even positions.
</p>
<h3>Output</h3>
<p>
	For each i = 1,...,d, your program should write to the i-th line of the output 
	file one word 'NO' if the i-th input expression cannot be transformed into any 
	expression of value k, and the smallest number of pairs of parentheses 
	necessary otherwise.
</p>
<h3>Example</h3>
<pre>Sample input:

5 
6 -4 
+5-4+5 
2 1 
+1 
4 1 
-1+1 
4 0 
-1+1 
4 -2 
-1+1 

Sample output:

1 
0 
NO 
0 
1 
</pre>