<p>Given a sequence of N (1 ¡Ü N ¡Ü 10,000) integers S<sub>1</sub>, ..., S<sub>N</sub> (0 ¡Ü S<sub>i</sub> &lt; 100,000), compute the number of increasing subsequences of S with length K (1 ¡Ü K ¡Ü 50 and K ¡Ü N); that is, the number of K-tuples i<sub>1</sub>, ..., i<sub>K</sub> such that 1 ¡Ü i<sub>1</sub> &lt; ... &lt; i<sub>K</sub> ¡Ü N and S<sub>i<sub>1</sub></sub> &lt; ... &lt; S<sub>i<sub>K</sub></sub>.</p>

<h3>Input</h3>
<p>The first line contains the two integers N and K. The following N lines contain the integers of the sequence in order.</p>

<h3>Output</h3>
<p>Print a single integer representing the number of increasing subsequences of S of length K, modulo 5,000,000.</p>

<h3>Example</h3>

<pre><b>Input:</b>
4 3
1
2
2
10

<b>Output:</b>
2
</pre>

<p>The two 3-tuples are (1, 2, 4) and (1, 3, 4), both corresponding to the subsequence 1, 2, 10.</p>