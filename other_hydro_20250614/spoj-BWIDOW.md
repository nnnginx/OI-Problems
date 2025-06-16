<p>
Black Widow has a collection of <strong>N</strong> (numbered 1 to N) Rings. She uses the rings to attack the enemies. She has decided to use one ring for distraction. She will first throw the distraction ring and then all the other rings will be thrown through it (one at a time). Each ring has an inner and outer radius. </p>

<p>A ring R1 will pass through ring R2 only if the outer radius of R1 is less than the inner radius of R2.</p>

<p>If she can chose a distraction ring from the given collection print the index of the ring (1-based), else print -1.</p>

<h3>Input</h3>
<p>The first line of the input contains an integer <strong>T</strong> denoting the number of test cases.<br> The first line of each test case contains a single integer <strong>N</strong> denoting the number of Rings.<br> Next <strong>N</strong> lines consists of Inner and Outer Radius of the ith Ring - <strong>r</strong>, <strong>R</strong>.</p>
<ul>
<li><strong>1</strong> ¡Ü <strong>T</strong> ¡Ü <strong>100</strong></li>
<li><strong>2</strong> ¡Ü <strong>N</strong> ¡Ü <strong>1000</strong></li>
<li><strong>1</strong> ¡Ü <strong>r</strong> &lt; <strong>R</strong> ¡Ü <strong>10<sup>7</sup></strong></li>
</ul>

<p>(<strong>Edited: </strong><b>r</b> and <b>R</b> are integer)

</p><h3>Output</h3>
<p>For each test case print the desired result in separate line.</p>
<h3>Example</h3>

<pre><strong>Input:</strong>
2
3
2 3
6 8
3 5
3
4 5
5 8
3 10

<strong>Output:</strong>
2
-1</pre>