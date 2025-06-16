<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">Sameen has:</span></span></p>
<ol>
<li><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">An array having N integers</span></span></li>
<li><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">Q friends</span></span></li>
</ol>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">His friends are curious about the array. So, each of his friends asks Sameen a question about the array. Every question is described by 3 integers: i, j and k. In reply to a question, Sameen has to say the ¡°k alternating sum¡± of the subarray starting at position i and ending at position j [1 based indexing]</span></span></p>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;"><br></span></span></p>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">¡°k alternating sum¡± of a subarray starting at position i and ending at position j can be calculated in the following way:</span></span></p>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">Add the first k numbers[starting from position i]</span></span></p>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">Subtract the second k numbers[starting from position i+k]</span></span></p>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">Add the third k numbers[starting from position i+2*k]</span></span></p>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">Subtract the fourth k numbers[starting from position i+3*k]</span></span></p>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">And so on till adding/subtracting the j-th number¡­</span></span></p>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">(j-i+1) will be divisible by k.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">[See sample Input/output and explanation section for more details]</span></span></p>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">Can you help Sameen in answering the questions?&nbsp;</span></span></p>
<h3>Input</h3>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">The first line of input contains two integers N and Q. The next line contains N integers, the numbers in the array. Then each of the following Q lines contains 3 integers i, j &amp; k.&nbsp;</span></span></p>
<h3>Output</h3>
<p><span style="font-size: small;"><span style="font-family: tahoma, arial, helvetica, sans-serif;">For each query output an integer in a separate line, the answer for that query. Queries should be answered in the order given in the input.&nbsp;</span></span></p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p><span style="font-size: small;">1 <span style="color: #222222;">¡Ü&nbsp;</span>k <span style="color: #222222;">¡Ü</span>&nbsp;100000</span></p>
<p><span style="font-size: small;">1 <span style="color: #222222;">¡Ü&nbsp;</span>&nbsp;N <span style="color: #222222;">¡Ü&nbsp;</span>&nbsp;100000</span></p>
<p><span style="font-size: small;">1 <span style="color: #222222;">¡Ü&nbsp;</span>&nbsp;Q <span style="color: #222222;">¡Ü&nbsp;</span>100000</span></p>
<p><span style="font-size: small;">-1000000000 <span style="color: #222222;">¡Ü&nbsp;</span>&nbsp;Value of a number in the array <span style="color: #222222;">¡Ü&nbsp;</span>1000000000</span></p>
<p><strong><span style="font-size: small;">(j-i+1) will be divisible by k. </span></strong><strong>&nbsp;</strong></p>
<p><strong>&nbsp;</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p><span style="font-size: small;">6 6</span></p><p><span style="font-size: small;">4 1 -2 -3 4 5</span></p><p><span style="font-size: small;">2 5 2</span></p><p><span style="font-size: small;">1 6 1</span></p><p><span style="font-size: small;">1 6 3</span></p><p><span style="font-size: small;">1 6 6</span></p><p><span style="font-size: small;">3 3 1</span></p><span style="font-size: small;">3 4 1</span></pre>
<pre><strong>Output:</strong>
<p><span style="font-size: small;">-2</span></p><p><span style="font-size: small;">3</span></p><p><span style="font-size: small;">-3</span></p><p><span style="font-size: small;">9</span></p><p><span style="font-size: small;">-2</span></p><span style="font-size: small;">1</span></pre>
<pre><p><strong>Explanation</strong>:</p><p><span style="font-size: small;">In the first query, the subarray is [ 1, -2, -3, 4].</span></p><p><span style="font-size: small;">So ¡°2 alternating sum¡± is equal to: [1-2]-[-3+4] = -2</span></p><p><span style="font-size: small;">For the second query, we get [4]-[1]+[-2]-[-3]+[4]-[5] = 3</span></p><p><span style="font-size: small;"><br></span></p><p><span style="font-size: small;">N.B: Dataset is huge. Use faster I/O method.<strong>&nbsp;</strong></span></p></pre>