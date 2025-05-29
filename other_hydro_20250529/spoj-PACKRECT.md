<p>Four rectangles are given.  Find the smallest enclosing (new) rectangle into which these four may be fitted without overlapping.  By smallest rectangle, we mean the one with the smallest area.</p>
<p>All four rectangles should have their sides parallel to the corresponding sides of the enclosing rectangle.</p>
<p>Rectangles may be rotated 90 degrees during packing.</p>
<p>There may exist several different enclosing rectangles fulfilling the requirements, all with the same area.  You must produce all such enclosing rectangles.</p>
<h3>Input</h3>
<p>Four lines, each containing two positive space-separated integers that represent the lengths of a rectangle's two sides.  Each side of a rectangle is at least 1 and at most 50.</p>
<h3>Output</h3>
<p>The output file contains one line more than the number of solutions. The first line contains a single integer:  the minimum area of the enclosing rectangles.  Each of the following lines contains one solution described by two numbers p and q with p&lt;=q.  These lines must be sorted in ascending order of p, and must all be different.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre>1 2
2 3
3 4
4 5
</pre>
<strong>Output:</strong><br><br>40 <br>4 10 <br>5 8</pre>