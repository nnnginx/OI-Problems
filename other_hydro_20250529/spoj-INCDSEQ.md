<p>Given a sequence of N (1 ¡Ü N ¡Ü 10,000) integers S<sub>1</sub>, ..., S<sub>N</sub> (0 ¡Ü S<sub>i</sub> &lt; 1,000,000,000), compute the number of distinct increasing subsequences of S with length K (1 ¡Ü K ¡Ü 50 and K ¡Ü N).</p>

<h3>Input</h3>
<p>The first line contains the two integers N and K. The following N lines contain the integers of the sequence in order.</p>

<h3>Output</h3>
<p>Print a single integer representing the number of distinct increasing subsequences of S of length K, modulo 5,000,000.</p>

<h3>Example</h3>

<pre><b>Input:</b>
4 3
1
2
2
10

<b>Output:</b>
1
</pre>

<p>The only increasing subsequence of length 3 is 1, 2, 10.</p>