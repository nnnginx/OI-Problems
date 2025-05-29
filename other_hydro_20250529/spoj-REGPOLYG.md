<p>A regular convex polygon is a polygon where each side has the same length, and all interior angles are equal and less than 180 degrees. A square, for example, is a regular convex polygon. You are given three points which are vertices of a regular convex polygon <em>R</em>; can you determine the minimum number of vertices that <em>R</em> must have?</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Input</span></span></strong></p>
<p>Each test case consists of three lines. Line <em>i</em> consists of two floating point values <em>x</em><sub><em>i</em></sub> and <em>y</em><sub><em>i</em></sub> (−10<sup>4</sup> ≤ <em>x</em><sub>1</sub>, <em>y</em><sub>1</sub> ≤ 10<sup>4</sup>) where (<em>x</em><sub><em>i</em></sub>, <em>y</em><sub><em>i</em></sub>) are the coordinates of a vertex of <em>R</em>. The coordinates are given with a precision of 10<sup>−6</sup>, i.e., they differ from the exact coordinates by at most 10<sup>−6</sup>. You may assume that for each test case the Euclidean distance between any two given points is at least 1, and <em>R</em> has at most 1000 vertices. The input will finish with a line containing the word <tt>END</tt>.</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Output</span></span></strong></p>
<p>For each test case, print one line with the minimum number of vertices that <em>R</em> must have.</p>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Sample Input</span></span></strong></p>
<pre class="verbatim">-1385.736326 -146.954822
430.000292 -2041.361203
1162.736034 478.316025
0.000000 4147.000000
-4147.000000 0.000000
0.000000 -4147.000000
END
</pre>
<p><br> <br> <strong><span style="color: black; "><span style="font-size: medium; ">Sample Output</span></span></strong></p>
<pre class="verbatim">3
4
</pre>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Adrian Kuegel</em></blockquote>