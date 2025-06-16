<p>A set of gears is installed on the plane. You are given the center coordinate and radius of each gear, which are all integer-valued. For a given source and target gear, indicate what happens to the target gear if you attempt to turn the source gear. Possibilities are: 
</p><ul>
	<li>The source gear cannot move, because it would drive some gear in the arrangement to turn in both directions.</li>
	<li>The source gear can move, but it is not connected to the target gear.</li>
	<li>The source gear turns the target gear, at a certain ratio.</li>
</ul>
If the source gear cannot move, give this result, even if the source and target gears are not connected.
<p></p>

<h3>Input</h3>
<p>Each input will consist of a single test case. Note that your program may be run multiple times on different inputs. The first line of input contains a single integer <strong>n</strong> (1 ¡Ü <strong>n</strong> ¡Ü 1,000), the total number of gears. Following this will be <strong>n</strong> lines, one per gear, containing the <strong>x</strong>, <strong>y</strong> (-10,000 ¡Ü <strong>x</strong>, <strong>y</strong> ¡Ü10,000) and <strong>r</strong> (1 ¡Ü <strong>r</strong> ¡Ü 10,000) values for the gear, where (<strong>x</strong>, <strong>y</strong>) is the position of the axle of the gear, and <strong>r</strong> is its radius. Assume that the teeth of the gears are properly designed, and accounted for in the radius, so that any gear will mesh with any other gear if (and only if) they are tangent to each other. The gears will never overlap.</p>
<h3>Output</h3>
<p>Output a single line, with the following content, based on the result: 
</p><ul>
	<li><tt>"-1"</tt> - if the source gear cannot move.</li>
	<li><tt>"0"</tt> - if the source gear can move but is not connected to the target. </li>
	<li><tt>"a b"</tt> - if the source gear moves the target gear, where <strong>a</strong> and <strong>b</strong> are two space-separated integers, and <strong>a</strong> : <strong>b</strong> is the ratio of source gear revolutions to target gear revolutions reduced to its lowest form (i.e. they have no common factor other than 1). 
	<ul>
		<li><strong>a</strong> is always positive.</li>
		<li>If the target turns in the same direction as the source, <strong>b</strong> is positive.</li>
		<li>If the target turns in the opposite direction as the source, <strong>b</strong> is negative.</li>
	</ul>
</li></ul><p></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
16&nbsp;<br>10 10 5 <br>20 10 5 <br>30 10 5 <br>40 10 5 <br>10 20 5 <br>20 20 5 <br>30 20 5 <br>40 20 5 <br>10 30 5 <br>20 30 5 <br>30 30 5 <br>40 30 5 <br>10 40 5 <br>20 40 5 <br>30 40 5 <br>40 40 5</pre>
<pre><strong>Output:</strong>
1 1</pre>