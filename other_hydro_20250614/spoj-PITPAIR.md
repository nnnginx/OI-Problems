<p>
	It is necessary to find a minimal integer value R which is equal to the length of the hypotenuse (the side opposite the right angle) of N non-identical rectangular triangles with integer lengths of sides. 
</p>

<h3>Input</h3>
<p>
	t - number of test cases [t &lt;= 100], than t lines follow, each line contains one integer - N, equal 
to the required number of different rectangular triangles. [1 &lt;= N &lt;= 2000]<br>
</p><h3>Output</h3>
<p>
	For each test case your program should output a number R in a separate line (R fits in a 64-bit integer), equal to the minimal integer value of a hypotenuse for which exactly N different rectangular triangles can be constructed; then in separate lines follow exactly N numbers equal to the shorter 
cathetus (side adjacent to the right angle) of each of the rectangular triangles, in ascending order. 

</p><h3>Example</h3>
<p>
</p><pre><b>Input:</b>
2
1
2

<b>Output:</b>
5
3
25
7
15
</pre>