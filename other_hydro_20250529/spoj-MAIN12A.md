<p>Everyone loves Swampy. Swampy the Alligator lives under the city and yearns for a more human like existence. Swampy recently learned a new self describing sequence. The sequence is described in blocks where each block has the same number and two consecutive blocks have consecutive numbers in them. To construct the sequence start with '1'. Now '1' means that the following block is of length 1. As '1' was chosen in previous block, therefore '2' is chosen for the current block making the sequence '12'. Now '2' means that the following block is of length 2. As '2' was chosen in previous block, therefore '3' is chosen for the current block making the sequence '1233'. Now '33' means that the following 2 blocks are of length 3. As '3' was chosen in previous block, therefore '4' is chosen for the current block making the sequence '1233444'. And the second '3' in the sequence appends '555' in the already generated sequence, making the sequence '1233444555'.</p>
<h3>Input</h3>
<p>First line of the input contains an integer T, the number of test cases. Then T test cases follow. Each test case consists of a single integer N.</p>
<h3>Output</h3>
<p>For each test case, print Case #X: S, where X is the test case number starting from 1, S is the Nth term of the sequence described above.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
1
2
3
4

<strong>Output:</strong>
Case #1: 1
Case #2: 2
Case #3: 3
Case #4: 3
</pre>
<p>Constraints: T &lt;= 10000 1 &lt;= N &lt;= 1000000</p>