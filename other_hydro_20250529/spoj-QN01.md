<h3 style="text-align: left;">Problem Statement</h3>
<p>You are given an array of n integers ( 0 &lt;= n &lt;= 1000 ). Find a contiguous subsequence of these numbers [ a<sub>i</sub>, a<sub>j</sub> ] ( 1 &lt;= i, j &lt;= n ), such that the Exclusive-OR of these numbers is maximum. ( That is,&nbsp; a<sub>i</sub> XOR a<sub>i+1</sub> XOR... a<sub>j</sub> should be maximum ).</p>
<p>&nbsp;</p>
<h3 style="text-align: left;">Input</h3>
<p>The test case contains exactly 2 lines of input.</p>
<p>The first line contains a single integer n ( 0 &lt;= n &lt;= 1000 ), the total number of integers in the sequence given to you.<br>The next line contains n space separated integers such that the ith integer denotes a<sub>i</sub>. ( 0 &lt;= a<sub>i</sub> &lt;= 10<sup>9</sup> ). Note that these integers need not necessarily be distinct.</p>
<p>&nbsp;</p>
<h3 style="text-align: left;">Output</h3>
<p>Output two lines. In the first line, print out the value of the maximum XOR.<br>In the second line, print out i and j with a space separating them, such that [ a<sub>i</sub>, a<sub>j</sub> ] ( both endpoints inclusive ) denotes the contiguous subsequence with the maximum XOR value.</p>
<p>In case there is more than one subsequence with the maximum XOR value, print out the pair ( i, j ) such that ( i, j ) is lexicographically smallest. ( Formally, we say that a pair ( a, b ) is lexicographically smaller than another pair ( c,d ) if and only if (i) a &lt; c or (ii) a=c and b &lt; d. )</p>
<p><strong><span style="text-decoration: underline;">NOTE</span></strong> : The subsequence must be non-empty, but may be allowed to contain just one integer. ( i.e, in this case, i = j )</p>
<p>&nbsp;</p>
<h3 style="text-align: left;">Example</h3>
<pre><strong>Input #1:</strong>
<br>1<br>4</pre>
<pre><span style="font-weight: bold;">Output #1:</span></pre>
<pre>4<br>1 1<br><br><strong><br></strong></pre>
<pre><strong>Input #2:</strong><br><br>3<br>1 2 3<br><br><strong>Output #2:</strong><br><br>3<br>1 2<br><strong><br><br>Explanation:</strong></pre>
<ol>
<li>In the first test case, since there is only one number, the maximum XOR would be simply the value of that number ( in this case, 4 ), and i = j = 1.</li>
<li>In the second test case, the maximum XOR value is 3, but there are 2 contiguous subsequences that define the same XOR value - (i) [ 1, 2 ] since 1 XOR 2 = 3 (ii) [ 3, 3 ] since this subsequence contains just the single integer 3.&nbsp;But since [ 1, 2 ] is lexicographically smaller than [ 3, 3 ], [ 1, 2 ] is the desired output.</li>
</ol>