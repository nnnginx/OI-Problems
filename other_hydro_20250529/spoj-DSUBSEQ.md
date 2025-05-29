<p>Given a string, count the number of distinct subsequences of it ( including empty subsequence ). For the uninformed, A subsequence of a string is a new string which is formed from the original string by deleting some of the characters without disturbing the relative positions of the remaining characters.
<br>For example, "AGH" is a subsequence of "ABCDEFGH" while "AHG" is not.

</p><h3>Input</h3>
<p>First line of input contains an integer T which is equal to the number of test cases. You are required to process all test cases. Each of next T lines contains a string s.

</p><h3>Output</h3>
<p>Output consists of T lines. Ith line in the output corresponds to the number of distinct subsequences of ith input string. Since, this number could be very large, you need to output ans%1000000007 where ans is the number of distinct subsequences.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
AAA
ABCDEFG
CODECRAFT


<b>Output:</b>
4
128
496
</pre>

<h3>Constraints and Limits</h3>
<p>T ¡Ü 100, length(S) ¡Ü 100000<br>
All input strings shall contain only uppercase letters.
</p>