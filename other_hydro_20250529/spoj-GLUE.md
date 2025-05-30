<p>
	Little Johnny decided he needed to stick an open metal box to the floor in the 
	hall of his parents' house, so that all guests coming in would trip on it. He 
	knew that as soon as his parents saw what he had done, they would try to remove 
	it, and he wasn't going to stand for this. So, he chose the strongest glue in his 
	possession and left lots of dabs of it on the floor (from our point of view, 
	these can be regarded as points). Now, the only question that remained was how 
	to stick the box onto the floor. Johnny is very particular about the way he 
	does this: the box is always stuck face down, so that it only touches the floor 
	on the four edges of the rectangle that forms its base. He would like each of 
	these edges to make contact with at least two dabs of glue. Furthermore, he 
	doesn't want any of the dabs to stay outside the box, since this would ruin the 
	fun (there is no way you can trip someone up, if you've glued them to the 
	floor, is there?).
</p>
<p>
	Obviously, Johnny can sometimes reach his objective in more than one way 
	(especially since he has prepared boxes of all possible dimensions for his act 
	of mischief). Depending on how he does this, a different section of floor will 
	be covered by the box. Determine in how many ways Johnny can choose the section 
	of floor to be covered by the box when gluing.
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	The first line of each test case contains positive integer n&lt;=10000 
	- the number of dabs of glue on the floor. The next n lines contain two 
	integers, x y (-15000&lt;=x,y&lt;=15000), representing the x and y coordinates 
	of the dabs (given in the order in which they were placed by Johnny ;).
</p>
<h3>Output</h3>
<p>
	For each test case output the number of different sections of floor Johnny may 
	choose to cover (possibly 0).
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1 
8 
1 0 
1 4 
0 3 
5 4 
5 0 
6 1 
6 3 
0 1 

<b><tt>Sample output:</tt></b>
2
</pre>