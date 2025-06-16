<p>
	A parliamentary election was being held in Byteland. Its enterprising and orderly citizens decided to limit the entire election campaign to a single dedicated wall, so as not to ruin the panorama with countless posters and billboards. Every politician was allowed to hang exactly one poster on the wall. All posters extend from top to bottom, but are hung at different points of the wall, and may be of different width. The wall is divided horizontally into sections, and a poster completely occupies two or more adjacent sections.
</p>
<p>
	With time, some of the posters were covered (partially or completely) by those of other politicians. Knowing the location of all the posters and the order in which they were hung, determine how many posters have at least one visible section in the end.
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test cases follow.
</p>
<p>
	Each test case begins with a line containing integer n - the number of posters (1 &lt;= n &lt;= 40000). Then n lines follow, the i-th (1 &lt;= i &lt;= n) containing exactly two integers l<sub>i</sub> r<sub>i</sub>, denoting the numbers of the leftmost and rightmost sections covered by the i-th poster (1 &lt;= l<sub>i</sub> &lt; r<sub>i</sub> &lt;= 10<sup>7</sup>). The input order corresponds to the order of hanging posters.
</p>
<h3>Output</h3>
<p>
	For each test case output a line containing one integer&nbsp;- the number of posters with visible sections.
</p>
<h3>Example</h3>
<pre><b>Sample input:</b>
1
5
1 4
2 6
8 10
3 4
7 10

<b>Sample output:</b>
4
</pre>
<p>
	An illustration of the sample input is given below.<br>
	<br>
	<img src="/content/adrian:sampleio.png" alt="The wall with posters">
</p>