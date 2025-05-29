Given an array <strong>A</strong> of <strong>N</strong> integers, you are required to solve <strong>Q</strong> queries. Each query consists of a positive integer <strong>V</strong> and a non-negative integer <strong>K</strong>. For each query, find out how many numbers in the array <strong>A</strong> have exactly <strong>K</strong> common one bits with the number <strong>V</strong>.

<br><br>

In other words, for each query, you need to calculate how many numbers are there in the array such that <strong>A<sub>i</sub></strong> &amp; <strong>V</strong> have exactly <strong>K</strong> bits set in its binary representation, where <strong>&amp;</strong> denotes the <i>bitwise AND</i> operation.

<br><br>

Note that since the input can be huge, they will be generated randomly using a pseudorandom generator, whose parameters will be given as input. Also for similar reasons, it is not required to output the result for every query, rather compute the sum of this value for all queries and output this sum. More specifically, for the <strong>i-th</strong> query, let <strong>C<sub>i</sub></strong> be the count of integers in <strong>A</strong> having exactly <strong>K</strong> common one bits with <strong>V<sub>i</sub></strong>. Then it is required to output the sum of all <strong>C<sub>i</sub></strong> only.

<br><br>

<h3>Input</h3>
The first line contains an integer <strong>T</strong>, denoting the number of test cases. Each test case contains six space separated integers in the order: <strong>seed, N, Q, mod_A, mod_V, mod_K</strong>. Afterwards, the input for each test case will be generated as described by the python code below.
<br><br>

<pre>def random():
   global seed
   seed = (seed * 997 + 29) % 2117566807
   return seed

A = [0 for _ in range(N)]

for i in range(N):
   A[i] = random() % mod_A

V = [0 for _ in range(Q)]
K = [0 for _ in range(Q)]

for i in range(Q):
   V[i] = random() % mod_V
   K[i] = random() % mod_K
</pre>

<br><br>

Note that the <strong>seed</strong> is a global variable which gets updated after each random call, with the initial value being given as input.

<h3>Constraints</h3>
<strong><li>1 ¡Ü T ¡Ü 25</li></strong>
<strong><li>1 ¡Ü N, Q ¡Ü 250000</li></strong>
<strong><li>0 ¡Ü seed &lt; 2117566807</li></strong>
<strong><li>1 ¡Ü mod_A, mod_V ¡Ü 250000</li></strong>
<strong><li>1 ¡Ü mod_K ¡Ü 19</li></strong>

<h3>Output</h3>
For each test case, output the case number followed by the required output. Please refer to the sample input/output section for more clarity of the format.

<h3>Sample Input</h3>
<pre>2
1 10 10 4 4 3
0 100 1000 10000 100000 10


</pre>

<h3>Sample Output</h3>
<pre>Case 1: 26
Case 2: 10260

</pre>

<h3>Explanation</h3>
For the first case:
<br><br>
<strong>A = [2, 3, 0, 1, 1, 2, 2, 3, 1, 0]</strong>
<br><br>
<strong>V = [2, 0, 3, 1, 0, 0, 2, 0, 0, 1]</strong>
<br><br>
<strong>K = [0, 2, 1, 1, 1, 2, 2, 0, 2, 2]</strong>
<br><br>
<strong>C = [5, 0, 6, 5, 0, 0, 0, 10, 0, 0]</strong>
<br><br>