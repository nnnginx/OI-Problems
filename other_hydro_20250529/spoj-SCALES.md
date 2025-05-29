<p>
	You are given scales for weighing loads. On the left side lies a single stone 
	of known weight W&lt;2<sup>N</sup>. You own a set of N different weights, 
	weighing 1, 2, 4, ..., 2<sup>N-1</sup> units of mass respectively. Determine 
	how many possible ways there are of placing some weights on the sides 
	of the scales, so as to balance them (put them in a state of equilibrium). 
	Output this value modulo a small integer D.
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case, the first line contains three integers: N L D, where N 
	denotes the number of weights at your disposal, L is the length of the binary 
	representation of number W, and D is the modulus (1&lt;= L&lt;= N&lt;= 1000000, 
	2&lt;= D&lt;=100). The second line contains the value of W, encoded in the 
	binary system as a sequence of exactly L characters 0 or 1 without separating 
	spaces.
</p>
<h3>Output</h3>
<p>
	For each test case, output a single line containing one integer - the calculated number of possible 
	weight placements, modulo D.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
2
6 4 6
1000
6 6 100
100110

<b><tt>Sample output:</tt></b>
3
5
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>