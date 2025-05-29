<p>Given an integer array of N integers, find the sum of bit differences in all the pairs that can be formed from array elements. Bit difference of a pair (x, y) is the count of different bits at the same positions in binary representations of x and y. For example, bit difference for 2 and 7 is 2. Binary representation of 2 is 010 and 7 is 111 (first and last bits differ in two numbers).</p>
<h3>Input</h3>
<p>Input begins with a line containing an integer <strong>T(1&lt;=T&lt;=100)</strong>, denoting the number of test cases. Then T test cases follow. Each test case begins with a line containing an integer <strong>N(1&lt;=N&lt;=10000)</strong>, denoting the number of integers in the array, followed by a line containing <strong>N</strong> space separated 32-bit integers.</p>
<h3>Output</h3>
<p>For each test case, output a single line in the format <strong>Case X: Y</strong>, where <strong>X</strong> denotes the test case number and <strong>Y</strong> denotes the sum of bit differences in all the pairs that can be formed from array elements modulo <strong>10000007</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
4
3 2 1 4

<strong>Output:</strong>
Case 1: 22
</pre>