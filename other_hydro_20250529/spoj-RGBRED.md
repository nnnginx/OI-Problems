<p>Given a color string consisting of primary colors only (Red, Green, Blue), any two adjacent colors can be combined to form the third color. Print the smallest possible length of the color string after all possible combinations.&nbsp;</p>
<h3>Input</h3>
<p>First line contains a positive integer T representing number of testcases.</p>
<p>Next line contains a number n denoting the size of color array.</p>
<p>Next line contains a n size color string</p>
<p>1 ¡Ü T ¡Ü 100</p>
<p>1 ¡Ü n ¡Ü 10<sup>5</sup></p>
<h3>Output</h3>
<p>Output minimum possible length of the final color string.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>3<br>RGB<br>4<br>RGBR</pre>
<pre><strong>Output:</strong><br>2<br>1</pre>
<pre><strong>Explanation:</strong><br>Example 1:<br>[RG]B ¡ú BB<br><br>Example 2:<br>[RG]BR ¡ú B[BR] ¡ú [BG] ¡ú R</pre>