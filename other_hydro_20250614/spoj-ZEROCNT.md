<p>Write down N integers 1, 2, ..., N in binary system on a paper, one per line, ignore all leading 0s:</p>
<p>1</p>
<p>10</p>
<p>11</p>
<p>100</p>
<p>101</p>
<p>110</p>
<p>111</p>
<p>...</p>
<p>Now on each line, consider all groups of consecutive 0s, index these group from 1. We will color all zeros in the 1st, (K+1)th, (2K+1)th, ... group, for K is a given integer.</p>
<p>For example: if a number in binary is: 1<span style="color: #ff0000;">0</span>1000111<span style="color: #ff0000;">00</span>110000, and K = 2. We have 4 groups of consecutive 0s, and we will color all zeros in the 1st and the 3rd group. So we will color 1 + 2 = 3 zeros in this line.</p>
<p>Given N and K. Compute total number of 0s we will color in the paper. (The paper is big enough to contain all numbers :D)</p>
<h3>Input</h3>
<p>Several lines, each line contains 2 integers: N and K separated by a single space. (1 &lt; N &lt; 2<sup>31</sup>, K &gt; 0)</p>
<h3>Output</h3>
<p>For each line in the input, print exactly 1 number on a single line which is the result of the corresponding test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>4 1<br>56 2<br><strong>Output:</strong><br>3<br>92</pre>