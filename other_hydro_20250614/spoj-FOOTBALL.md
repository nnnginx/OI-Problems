<p>
	Eric has a classic football that is made of 32 pieces of leather: 12 black 
	pentagons and 20 white hexagons. Each pentagon adjoins 5 hexagons and each 
	hexagon adjoins 3 pentagons and 3 hexagons. Eric drew a polygon (i.e. a closed 
	line without intersections) along the edges of the pieces. The polygon divided 
	the ball into two parts and Eric painted one of them green.
</p>
<img src="/content/adrian:FOOTBALL.png" alt="Eric's football">
<p>
	He is curious if given a description of the polygon you are able to compute the 
	number of black, white and green pieces?
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads the description of a polygon,
		</li><li>
		computes the number of black, white and green pieces,
		</li><li>
			writes the result.</li>
	</ul>
</div>
<p>
	Contest note: the first accepted solution will be awarded with the original 
	football used for preparing the problem, signed by Eric, the author of the 
	problem!
</p>
<p>
	SPOJ note: the first accepted solution will be awarded some other sphere, 
	without anybody's signatures, sent in PNG format to the author's email address 
	[the offer is invalid, the sphere has already  been presented to Robin Nittka, University of Ulm, Germany].
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case, the first line of the input contains one integer n being 
	the number of vertices of the polygon. The second line of the input contains n 
	integers a<sub>1</sub>, a<sub>2</sub>,..., a<sub>n</sub> separated by single 
	spaces. Integer a<sub>i</sub> (equal 1 or 2) is the number of green pieces 
	adjoining the i-th vertex of the polygon. The side of the polygon connecting 
	the n-th and the first vertex always lies between two hexagons.
</p>
<h3>Output</h3>
<p>
	For each test case the first and only line of the output contains three 
	integers b, w and g - the numbers of black, white and green pieces 
	respectively.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
21 
1 2 1 2 1 2 1 1 1 2 2 1 1 1 1 2 2 2 1 1 1 

<b><tt>Sample output:</tt></b>
11 15 6 
</pre>