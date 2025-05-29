<p>Find the number of strings of length ¡°N¡± made up of only 3 characters ¨C a, b, c such that ¡°a¡± occurs at least ¡°min_a¡± times and at most ¡°max_a¡± times, ¡°b¡± occurs at least ¡°min_b¡± times and at most ¡°max_b¡± times and ¡°c¡± occurs at least ¡°min_c¡± times and at most ¡°max_c¡± times. Note that all permutations of same string count as 1, so ¡°abc¡± is same as ¡°bac¡±.</p>
<h3>Input</h3>
<p>First line gives T, the number of test cases.</p>
<p>Each test case has an integer ¡°N¡± on first line.</p>
<p>Next line contains 2 integers, min_a and max_a.</p>
<p>Next line contains 2 integers, min_b and max_b.</p>
<p>Next line contains 2 integers, min_c and max_c.</p>
<h3>Output</h3>
<p>Output T lines, each containing the required answer modulo 10^9+7.</p>
<h3>Constraints</h3>
<p>1&lt;=T&lt;=1000<br> 1&lt;=N&lt;=10^9<br> 1&lt;=min_a&lt;= max_a&lt;=10^9</p>
<p>1&lt;=min_b&lt;= max_b&lt;=10^9</p>
<p>1&lt;=min_c&lt;= max_c&lt;=10^9</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>1</p><p>3</p><p>1 1</p><p>1 1</p><p>1 1</p>
<strong>Output:</strong>
1</pre>