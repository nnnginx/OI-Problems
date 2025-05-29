<p>Given a string <strong>S</strong> which contains only digit-characters. How many  subsequences can be obtained from S such that every digit is strictly  greater than all previous digits in that subsequence.<br>As for example if S=7598 then there are 8 subsequences which follow  the above constraint. These are 7,5,9,8,79,78,59,58. Notice that 7598 is  not a required subsequence because 7&gt;5 and 9&gt;8.</p>
<p>Note: A subsequence is a sequence that can be derived from another  sequence by deleting some elements without changing the order of the  remaining elements.</p>
<h3>Input</h3>
<p>Input starts with an integer&nbsp;<strong>T (¡Ü 1000)</strong>, denoting the number of test cases. Each case contains a string <strong>S</strong>. The length of S does not exceed <strong>10000</strong>. S does not contain any leading zeros.</p>
<h3>Output</h3>
<p>For each case, print the a string(without quotes) <strong>"Case i: "</strong> follwed by number of subsequences where "i" is test case number. Answer may be very large, so output it&nbsp;<strong>modulo 10^9+7</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>2<br>4<br>7598

<strong>Output:</strong>
Case 1: 1<br>Case 2: 8</p><p>For small constraints: <strong>www.spoj.com/problems/SUBP/</strong></p></pre>