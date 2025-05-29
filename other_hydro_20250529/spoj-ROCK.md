<p>
	A manufacturer of sweets has started production of a new type of 
	sweet called <em>rock</em>. Rock comes in sticks composed of  
	one-centimetre-long segments, some of which are sweet, and the rest are sour. 
	Before sale, the rock is broken up into smaller pieces by splitting it at the 
	connections of some segments.
</p>
<p>Today's children are very particular about what they eat, and they will only buy 
	a piece of rock if it contains more sweet segments than sour ones. Try to 
	determine the total length of rock which can be sold after breaking 
	up the rock in the best possible way.
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case, the first line of input contains one integer N - the length 
	of the stick in centimetres (1&lt;=N&lt;=200). The next line is a sequence of N 
	characters '0' or '1', describing the segments of the stick from the left end 
	to the right end ('0' denotes a sour segment, '1' - a sweet one).
</p>
<h3>Output</h3>
<p>
	For each test case output a line with a single integer: the total length of 
	rock that can be sold after breaking up the rock in the best possible way.
</p>
<h3>Example</h3>
<pre><b>Sample input:</b>
2
15
100110001010001
16
0010111101100000

<b>Sample output:</b>
9
13
</pre>