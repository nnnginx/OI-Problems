Given a positive integer <strong>N</strong>, consider any permutation of all the numbers from <strong>1</strong> to <strong>N</strong>. It is required to create two partitions, <strong>P<sub>1</sub></strong> and <strong>P<sub>2</sub></strong>, from these numbers such that <strong>|sum(P<sub>1</sub>) ¨C sum(P<sub>2</sub>)|</strong> is minimum, where <strong>sum(X)</strong> denotes the summation of all the numbers in partition <strong>X</strong>. A partition is defined to be a non-empty subset of the permutation. In other words, find the minimum absolute difference between the summation of all the numbers in each partition. Note that you cannot leave out any number, every number from <strong>1</strong> to <strong>N</strong> must be part of exactly one partition.
<br><br>

<h3>Input</h3>
The first line contains an integer <strong>T</strong>, denoting the number of test cases. Each of the next subsequent <strong>T</strong> lines contain a positive integer <strong>N</strong>.
<br><br>

<h3>Constraints</h3>
<strong><li>1 ¡Ü T ¡Ü 1000</li></strong>
<strong><li>2 ¡Ü N ¡Ü 10<sup>9</sup></li></strong>

<h3>Output</h3>
For each test case, first print the case number followed by the minimum absolute difference.

<h3>Sample Input</h3>
<pre>5
2
3
4
5
6
</pre>

<h3>Sample Output</h3>
<pre>Case 1: 1
Case 2: 0
Case 3: 0
Case 4: 1
Case 5: 1
</pre>

<h3>Challenge</h3>
Try the harder version here:
<br><br>
<a href="https://www.spoj.com/problems/BPM2/">Bipartite Permutation (Hard)</a>