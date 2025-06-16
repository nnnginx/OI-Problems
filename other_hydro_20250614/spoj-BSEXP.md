<p>Problem Statement is easy, for a given number <em>N</em>, you have to print the <em>base B</em> such that if we write <em>N</em> in base <em>B</em> then it would contain most 0's at the end.</p>
<p>If more then one such <em>base</em> exist, which satisfy the given condition then print the smallest such base.</p>
<h3>Input</h3>
<p>The first line of the input consist of a single integer number <em>t</em> which determines the number of tests.</p>
<p>In each of next <em>t</em> lines there is a single integer number <em>N</em>.</p>
<h4>Constraints</h4>
<ul>
<li>0 &lt; t ¡Ü 10<sup>5</sup></li>
<li>2 ¡Ü N ¡Ü 10<sup>12</sup></li>
</ul>
<h3>Output</h3>
<p>Output contains one line with one integer <em>B</em> such that <em>N</em> written in base <em>B</em> has the most zeros at the end and is the smallest <em>B</em> with this property.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
72
18
<strong>Output:</strong>
2
3
</pre>
<h3>Explanation</h3>
<p>The answer for N=72 is B=2, because 72=1001000<sub>2</sub> (72 written in base 2) has 3 zeros at the end.</p>
<p>Using base 3, we only get 2 zeroes at the end (because 72=2200<sub>3</sub>),</p>
<p>using base 6 would also give us 2 zeros, and no other base would give us more than 1 zero</p>
<p>&nbsp;</p>
<pre>For 18, 18=10010<sub>2</sub> and 18=200<sub>3</sub> so answer will be 3.</pre>
<p>&nbsp;</p>
<pre><strong>Note:</strong>Testcase are regenerated on 23 June 2020.</pre>
<pre>As rejudge is disabled by SPOJ please submit your code again.</pre>