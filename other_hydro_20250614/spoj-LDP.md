<p>Most of the programmers like the problem description to be as short as possible, right? I also never like the problem description to be so narrative.</p>
<p>In this problem, you will be given an array <em>a</em> of n integers. If we multiply all the numbers of the array then we will get a result. Suppose the result is <em>K</em>.</p>
<p>&nbsp;</p>
<p>let's introduce another list of all the common multiples of an array as <em>cmp</em>. Definitely,&nbsp;the list has an infinite number of elements.</p>
<p>&nbsp;</p>
<p>Suppose, we have an array <em>a</em>&nbsp;= {2, 3, 6}. The result of multiplication of 2, 3 and 6 is 36. So <em>K</em> = 36.</p>
<p>The 1st common&nbsp;multiple of <em>a </em>is 6, the 2nd common multiple is 12, 3rd is 18, and so on.</p>
<p>So the list,&nbsp;<em>cmp = {6, 12, 18, 24, 30, 36, 42, ....... }.</em></p>
<p>&nbsp;</p>
<p>Now the question is what the position of <em>K&nbsp;in the&nbsp;cmp list</em>? (1-based indexing)</p>
<p>As the result can be very big, you have to print <em>K</em> % <em>1000000009</em>(<em>10<sup>9</sup> + <em>9)</em></em>, where % is modulo operator.</p>
<p>Note: In the above-described example, the position&nbsp;of&nbsp; <em>K </em>is 6. (<em>cmp<sub>6</sub>&nbsp;= K = 36).</em></p>
<h3>Input</h3>
<p>The first line of the input will be <em>n</em>, the number of elements in the array.</p>
<p>In the next line, <em>n</em> elements of the array <em>a<sub>1</sub>, <em>a<sub>2</sub>, <em>a<sub>3</sub> ... <em>a<sub>n</sub></em> will be given.</em></em></em></p>
<p><em><em> </em></em></p>
<h4>Constraints</h4>
<ul>
<li>0 &lt; n ¡Ü 10<sup>5</sup></li>
<li>0 &lt; <em>a<sub>i</sub></em> ¡Ü 10<sup>9</sup>(1 ¡Ü <em>i</em> ¡Ü n)</li>
</ul>
<h3>Output</h3>
<p>Print a single integer, the result of the problem described above with a new line.</p>
<h3>Example</h3>
<pre>		<strong>Input:</strong>
		3
		6 10 8
		<strong>Output:</strong>
		4
	</pre>
<p>&nbsp;</p>