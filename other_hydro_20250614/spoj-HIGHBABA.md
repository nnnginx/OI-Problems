<p>A spiritual baba in Banani claims that, given two strings he can check if one string is available in another string as sub-sequence and not only that, he can even tell the minimum sub-array in which that sub-sequence exists. Now your friend wants to know if that spiritual baba is fraud or not. So, he wants you to make an application for him.</p>
<p>You are given two strings A &amp; B. Now, find the minimum length sub-array of string ¡¯A¡¯ which contains the sub-sequence (string ¡®B¡¯). If such sub-sequence cannot be found, print -1.</p>
<p><strong>Subsequence:</strong> suppose a string ¡°abcdef¡± is given. Here, ¡±abcdef¡±, ¡°abf¡±, ¡°def¡±, ¡°bce¡±, ¡°a¡± are some example of sub-sequence of this string. But strings like ¡°fea¡± and ¡°dc¡± are not.</p>
<h3>Input</h3>
<p>The first line of the input contains an integer <strong>T (1 &lt;= T &lt;= 100)</strong> number of test cases. For each test case, two strings <strong>A (1 &lt;= N &lt;= 2500)</strong> and <strong>B (1 &lt;= M &lt;= 80)</strong> are given, each containing small letter English alphabet. Here N is length of string <strong>A</strong> and <strong>M</strong> is length of string <strong>B</strong>. Cases are separated by blank lines in input file.</p>
<h3>Output</h3>
<p>Output the case number and the expected answer for each test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
aabbaaccanbbbncc
abc

objectorientedprogramming
ii

<strong>Output:</strong>
Case 1: 6
Case 2: 15
</pre>