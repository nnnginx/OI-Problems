<p>Let a given sequence S (of length n) of positive integers be called x-medial (where x is a positive integer) if:</p>
<ol>
<li>n is odd, and the median of the sequence (the ((n+1)/2)<sup>th</sup>&nbsp;largest term)&nbsp;equals x. <strong>OR</strong></li>
<li>n is even, and both the central terms ( (n/2)<sup>th</sup>&nbsp;largest and (n/2+1)<sup>th</sup>&nbsp;largest) are equal to x.</li>
</ol>
<p>Given a sequence A (of length N) of positive integers and an integer k, find out how many of its sub-sequences are k-medial.</p>
<p>A sub-sequence of A is any sequence {A[i], A[i+1], A[i+2]... , A[j]}, where 0 ¡Ü i ¡Ü j &lt; N.</p>
<h3>Input</h3>
<p>The first line contains T (T¡Ü15), the number of test cases.</p>
<p>Each test case consists of 2 lines. The first line contains the numbers N (1¡ÜN¡Ü10<sup>5</sup>) and k (1¡Ük¡Ü10<sup>9</sup>), seperated by a single space.</p>
<p>The next line contains the sequence A (N terms, each ¡Ü 10<sup>9</sup>,&nbsp;&nbsp;seperated by single spaces between them).</p>
<h3>Output</h3>
<p>Output T lines, each containing a single integer, equal to the number of k-medial sub-sequences.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>3 5</pre>
<pre>17 5 2</pre>
<pre>5 2</pre>
<pre>1 2 2 3 7</pre>
<pre><strong>Output:</strong>
2</pre>
<pre>7</pre>