<p style="margin-bottom: 0cm; line-height: 100%;">Problem statement:</p>
<p style="margin-bottom: 0cm; line-height: 100%;">&nbsp;</p>
<p style="margin-bottom: 0cm; line-height: 100%;">You are given two DNA sequences A and B. It is said that these two DNA sequences are related if there exists a non-decreasing sequence C of the same length, such that C<sub>i </sub><strong>= </strong>A<sub>i</sub> or C<sub>i</sub> = B<sub>i</sub>. Find if the given sequences are related.</p>
<p style="margin-bottom: 0cm; line-height: 100%;">&nbsp;</p>
<p style="margin-bottom: 0cm; line-height: 100%;">Input format:</p>
<p style="margin-bottom: 0cm; line-height: 100%;">The first line contains an integer, T, the number of test cases.</p>
<p style="margin-bottom: 0cm; line-height: 100%;"><a name="MathJax-Span-199"></a><a name="MathJax-Span-198"></a><a name="MathJax-Span-197"></a><a name="MathJax-Element-34-Frame"></a><a name="MathJax-Span-202"></a><a name="MathJax-Span-201"></a><a name="MathJax-Span-200"></a><a name="MathJax-Element-35-Frame"></a><a name="MathJax-Span-205"></a><a name="MathJax-Span-204"></a><a name="MathJax-Span-203"></a><a name="MathJax-Element-36-Frame"></a> For each test case:<br>The first line contains an integer,<span style="display: inline-block; border: none; padding: 0cm;"><span style="font-family: 'MathJax Math-italic';"><span style="font-size: 16pt;">N</span></span></span>, the length of the DNA sequence.<br>The second line contains a sequence of space-separated integers describing species <span style="display: inline-block; border: none; padding: 0cm;"><span style="font-family: 'MathJax Math-italic';"><span style="font-size: 16pt;">A</span></span></span>.<br>The third line contains a sequence of space-separated integers describing species <span style="display: inline-block; border: none; padding: 0cm;"><span style="font-family: 'MathJax Math-italic';"><span style="font-size: 16pt;">B</span></span></span>.</p>
<p style="margin-bottom: 0cm; line-height: 100%;">&nbsp;</p>
<p style="margin-bottom: 0cm; line-height: 100%;"><span style="display: inline-block; border: none; padding: 0cm;"><span style="color: #000000;"><span style="font-family: 'Liberation Serif', serif;"><span style="font-size: 13pt;"><strong>Output Format</strong></span></span></span></span></p>
<p style="margin-bottom: 0cm; line-height: 100%;"><span style="display: inline-block; border: none; padding: 0cm;"><span style="color: #000000;"><span style="font-family: 'Liberation Serif', serif;"><span style="font-size: 13pt;">On a new line for each test case, print </span></span></span></span><span style="color: #000000;"><span style="font-family: 'Liberation Serif', serif;"><span style="font-size: 13pt;"><strong>YES </strong></span></span></span><span style="color: #000000;"><span style="font-family: 'Liberation Serif', serif;"><span style="font-size: 13pt;">if a non-decreasing sequence of the same length can be found or </span></span></span><span style="color: #000000;"><span style="font-family: 'Liberation Serif', serif;"><span style="font-size: 13pt;"><strong>NO </strong></span></span></span><span style="color: #000000;"><span style="font-family: 'Liberation Serif', serif;"><span style="font-size: 13pt;">if it cannot.</span></span></span></p>
<p style="margin-bottom: 0cm; line-height: 100%;">&nbsp;</p>
<p style="margin-bottom: 0cm; line-height: 100%;"><span style="display: inline-block; border: none; padding: 0cm;"><span style="font-family: 'Liberation Serif', serif;"><span style="font-size: 13pt;">Constraints:</span></span></span></p>
<p style="margin-bottom: 0cm; line-height: 100%;"><a name="MathJax-Element-37-Frame"></a><a name="MathJax-Span-206"></a><a name="MathJax-Span-207"></a><a name="MathJax-Span-208"></a><a name="MathJax-Span-209"></a><a name="MathJax-Span-210"></a><a name="MathJax-Span-211"></a><a name="MathJax-Span-212"></a><a name="MathJax-Span-219"></a><a name="MathJax-Span-220"></a><a name="MathJax-Element-39-Frame"></a><a name="MathJax-Span-222"></a><a name="MathJax-Span-223"></a><a name="MathJax-Span-224"></a><a name="MathJax-Span-225"></a><a name="MathJax-Span-226"></a><a name="MathJax-Span-227"></a><a name="MathJax-Span-228"></a><a name="MathJax-Span-229"></a><a name="MathJax-Span-230"></a><a name="MathJax-Span-231"></a><a name="MathJax-Span-232"></a><a name="MathJax-Span-233"></a><a name="MathJax-Span-234"></a><a name="MathJax-Span-237"></a><a name="MathJax-Span-238"></a><a name="MathJax-Span-239"></a> <span style="font-family: 'Liberation Serif', serif;"><span style="font-size: 16pt;">1 ¡Ü T ¡Ü 5</span>&nbsp;<br><span style="font-size: 16pt;">1 &lt;= N &lt;= 10 ^ 5</span><br><span style="font-size: 16pt;">0 ¡Ü A</span><span style="font-size: 11pt;">i</span><span style="font-size: 16pt;">, B</span><span style="font-size: 11pt;">i </span><span style="font-size: 16pt;">¡Ü </span><span style="font-size: 16pt;">10 ^ 10</span></span></p>
<p style="margin-bottom: 0cm; line-height: 100%;">&nbsp;</p>
<p style="margin-bottom: 0cm; line-height: 100%;">&nbsp;</p>
<p style="margin-bottom: 0cm; line-height: 100%;">&nbsp;</p>
<p style="margin-bottom: 0cm; line-height: 100%;"><span style="display: inline-block; border: none; padding: 0cm;"><span style="font-family: 'Liberation Serif', serif;"><span style="font-size: 13pt;">Sample input:</span></span></span></p>
<pre><br>
</pre>
<pre>3</pre>
<pre>3</pre>
<pre>1 2 3</pre>
<pre>4 4 4</pre>
<pre>3</pre>
<pre>3 2 1</pre>
<pre>6 5 4</pre>
<pre>2</pre>
<pre>1 0</pre>
<pre>10 2</pre>
<pre><br>
</pre>
<pre>Sample Output:</pre>
<pre>YES</pre>
<pre>NO</pre>
<pre>YES</pre>