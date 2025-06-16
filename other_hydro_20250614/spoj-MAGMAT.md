<p>A magical matrix I<sub>x</sub> is obtained by right shifting an Identity matrix of size q exactly n times in a circular manner.</p>
<p><img src="file://1XGRyTKV.png" alt="" width="363" height="67"></p>
<p>q in the above example is 3.</p>
<p>Bob is very fond of such matrices so he embeds them in his m x n matrix where each cell represents the value x of I<sub>x </sub>that he embeds. Now he is wondering if he can find a loop connecting 1's across this new matrix such that: Exactly 6 1s are connected and every time&nbsp;a 1 is selected it must be from the same column or row (in an alternate manner). Initially, we can choose any element having 1 and next can choose any element within same row or column. Next element must be from the same column if previously it was from the same row hence every successive selection must be in an alternate manner.</p>
<p><img src="file://KBa6WXCq.png" alt="" width="573" height="198"></p>
<p>Two such paths are&nbsp;shown in the above image (q is taken 3). A path is considered unique if it has at least one node different in it.</p>
<h3>Input</h3>
<p>The first line of each input test case contains 3 integers m (1 &lt; m ¡Ü 12), n (1 &lt; n ¡Ü 6) &amp; q (1 &lt; q ¡Ü 100)</p>
<p>Next lines contain the matrix having m rows and n columns</p>
<h3>Output</h3>
<p>Print an integer which tells the number of such paths possible</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 3 3
1 2 3
4 5 6
7 8 9</pre>
<pre><strong>Output:</strong>
18</pre>