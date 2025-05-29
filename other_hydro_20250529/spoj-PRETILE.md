<p>You are given a string S with N (1 ¡Ü N ¡Ü 100,000) characters from 'A' to 'Z', inclusive. For an integer L between 1 and N, inclusive, we define match (L) as the length of the longest prefix of S that can be tiled by the length-L prefix of S; more specifically, match (L) is the smallest 0-based index k such that S [k] ¡Ù S [k mod L], or N if no such k exists. For example, when S = "ABCAB", match (1) = 1, match (3) = 5, and match (4) = 4. Compute the sum match (1) + match (2) + ... + match (N).

</p><h3>Input</h3>
<p>The first line contains the integer T (1 ¡Ü T ¡Ü 10), the number of tests. For each test, there is a single line containing the string S.</p>

<h3>Output</h3>
<p>For each test case, print a single line containing one integer: the value of match (1) + match (2) + ... + match (N).</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
ABCAB
ZZZZZZ

<b>Output:</b>
17
36
</pre>

<p>For the first test case, match (1) + match (2) + match (3) + match (4) + match (5) = 1 + 2 + 5 + 4 + 5 = 17. For the second, the sum is equal to 6 * 6 = 36.</p>

<b>Warning: large input/output data.</b>