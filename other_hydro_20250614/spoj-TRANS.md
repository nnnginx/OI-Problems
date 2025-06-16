<p>
	You are given two short sequences of numbers, X and Y. Try to determine the 
	minimum number of steps of transformation required to convert sequence X into 
	sequence Y, or determine that such a conversion is impossible.
</p>
<p>
	In every step of transformation of a sequence, you are allowed to replace 
	exactly one occerunce of one of its elements by a sequence of 2 
	or 3 numbers inserted in its place, according to a rule specified in the input 
	file.
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case, the first line of input contains four integers - N, M, U, V 
	(1&lt;=N,M&lt;=50). The next two lines of input contain sequences X and Y, 
	consisting of N and M integers respectively. The next U lines contain three 
	integers: <i>a b c</i> each, signifying that integer <i>a</i> can be converted 
	to the sequence <i>b c</i> in one step of transformation. The next V-U lines 
	contain four integers: <i>a b c d</i> each, signifying that integer <i>a</i> can 
	be converted to the sequence <i>b c d</i> in one step of transformation. With 
	the exception of N and M, all integers provided at input are positive and do 
	not exceed 30.
</p>
<p>
	The format of one set of input data is illustrated below.<br>
	<img src="/content/adrian:TRANS.png">
</p>
<h3>Output</h3>
<p>For each test case output -1 if it is impossible to convert sequence X into 
	sequence Y, or the minimum number of steps required to achieve this conversion 
	otherwise.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
3 10 2 3
2 3 1
2 1 1 2 2 1 2 1 2 1
3 1 2
3 3 3
3 1 3 2

<b><tt>Sample output:</tt></b>
6
</pre>