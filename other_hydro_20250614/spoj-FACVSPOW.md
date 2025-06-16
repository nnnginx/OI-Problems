<p>Consider two integer sequences <b>f(n) = n!</b> and <b>g(n) = a<sup>n</sup></b>, where <b>n</b> is a positive integer. For any integer <b>a &gt; 1</b> the second sequence is greater than the first for a finite number of values. But starting from some integer <b>k</b>, <b>f(n)</b> is greater than <b>g(n)</b> for all <b>n &gt;= k</b>. You are to find the least positive value of <b>n</b> for which <b>f(n) &gt; g(n)</b>, for a given positive integer <b>a &gt; 1</b>.

</p><h3>Input</h3>
<p>The first line of the input contains number <b>t</b> ¨C the amount of tests. Then <b>t</b> test descriptions follow. Each test consist of a single number <b>a</b>.

</p><h3>Constraints</h3>
<p>1 &lt;= <b>t</b> &lt;= 100000<br>
2 &lt;= <b>a</b> &lt;= 10<sup>6</sup></p>

<h3>Output</h3>
<p>For each test print the least positive value of <b>n</b> for which <b>f(n) &gt; g(n)</b>.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
2
3
4

<b>Output:</b>
4
7
9
</pre>