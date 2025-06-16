<p>A cat is chasing a mouse in a rectangular room which contains some obstacles. The cat and mouse move according to the following rules:</p>
<ol>
<li>The cat and mouse move in turns, in alternating fashion. The cat starts. </li>
<li>Both the cat and the mouse can only move to a location that does not contain an obstacle, and that is horizontally, vertically, or diagonally adjacent to their current location. Staying in the same location is always a valid move. </li>
<li>Neither the cat nor the mouse can move beyond the border of the room. </li>
<li>The cat is always aware of the location of the mouse, and vice versa. </li>
</ol>
<p>Given the description of the room, and the starting positions of the cat and of the mouse, your task is to decide whether the mouse can avoid the cat forever or not.</p>
<h3>Input</h3>
<p>The first line of the input contains <em>T</em> (<em>1 ¡Ü T ¡Ü 10</em>), the number of test cases.  Then <em>T</em> test cases follow, separated by blank lines.  Each test case consists of a line describing the length of the two sides of the room, <em>R</em> and <em>C</em> (<em>1 ¡Ü R ¡Ü 10</em>, <em>1 ¡Ü C ¡Ü 10</em>), followed by a description of the room. The room is given as a matrix of <em>R</em> rows and <em>C</em> columns, where each entry of the matrix is either:</p>
<ul>
<li>a dot (<tt>.</tt>), if the corresponding location is free of obstacles, </li>
<li>a hash sign (<tt>#</tt>), if the corresponding location contains an obstacle, </li>
<li>an <tt>m</tt>, if the corresponding location is the starting position of the mouse, </li>
<li>a <tt>c</tt>, if the corresponding location is the starting position of the cat. </li>
</ul>
<p>The starting position of the cat and the starting position of the mouse are always different. Clearly, the starting positions are free of obstacles.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>The output consists of one line for each test case, containing the string <tt>mouse</tt> if the mouse can avoid the cat forever, and the string <tt>cat</tt> otherwise.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>2
3 3
#c#
.#m
#.#

3 3
#c#
.#.
#m#
</pre>
<p><strong>Output</strong></p>
<pre>cat
mouse
</pre>