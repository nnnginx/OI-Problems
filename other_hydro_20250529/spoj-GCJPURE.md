<h3>Problem</h3>
<p>&nbsp;</p>
<blockquote><em>Pontius</em>: You know, I like this number 127, I don't know why.<br> 
<em>Woland</em>: Well, that is an object so pure. You know the <em>prime numbers</em>.<br> 
<em>Pontius</em>: Surely I do. Those are the objects possessed by our  ancient masters hundreds of years ago. Oh, yes, why then? 127 is indeed a  prime number as I was told.<br> <em>Woland</em>: Not... only... that. 127 is the 31st prime number; then,  31 is itself a prime, it is the 11th; and 11 is the 5th; 5 is the 3rd;  3, you know, is the second; and finally 2 is the 1st.<br> <em>Pontius</em>: Heh, that is indeed... purely prime.<br></blockquote>
<p>The game can be played on any subset <code>S</code> of positive integers. A number in <code>S</code> is considered pure with respect to <code>S</code> if, starting from it, you can continue taking its rank in <code>S</code>, and get a number that is also in <code>S</code>, until in finite steps you hit the number 1, which is not in <code>S</code>.</p>
<p>When <strong>n</strong> is given, in how many ways you can pick <code>S</code>, a subset of {2, 3, ..., n}, so that <strong>n</strong> is pure, with respect to <code>S</code>? The answer might be a big number, you need to output it modulo 100003.</p>

<h3>Input</h3>
<p>The first line of the input gives the number of test cases, <strong>T</strong>.  <strong>T</strong> lines follow.  Each contains a single integer <strong>n</strong>.</p>

<h3>Output</h3>
<p>For each test case, output one line containing "Case #x: y", where x is  the case number (starting from 1) and y is the answer as described  above.</p>

<h3>Limits</h3>
<p><strong>T</strong> ¡Ü 200.</p>
<p>2 ¡Ü <strong>n</strong> ¡Ü 500.</p>

<h3>Sample</h3>
<pre><strong>Input:</strong>
2
5
6

<strong>Output:</strong>
Case #1: 5
Case #2: 8</pre>

<p>(All problem statements, input data and contest analyses from google code jam are     licensed under the     <a href="http://creativecommons.org/licenses/by/3.0/">Creative Commons Attribution License</a>.)</p>