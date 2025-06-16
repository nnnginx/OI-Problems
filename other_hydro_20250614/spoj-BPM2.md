Given a positive integer <strong>N</strong>, consider any permutation of all the numbers from <strong>1</strong> to <strong>N</strong>. It is required to create two partitions, <strong>P<sub>1</sub></strong> and <strong>P<sub>2</sub></strong>, from these numbers such that <strong>|sum(P<sub>1</sub>) ¨C sum(P<sub>2</sub>)|</strong> is minimum, where <strong>sum(X)</strong> denotes the summation of all the numbers in partition <strong>X</strong>. A partition is defined to be a non-empty subset of the permutation. In other words, find the minimum absolute difference between the summation of all the numbers in each partition. Note that you cannot leave out any number, every number from <strong>1</strong> to <strong>N</strong> must be part of exactly one partition.

<br><br>

To add a little bit more of spice, also find the lexicographically smallest partition <strong>P<sub>1</sub></strong> such that <strong>|sum(P<sub>1</sub>) ¨C sum(P<sub>2</sub>)|</strong> is minimum. To make your life easier, you don¡¯t need to output the entire sequence, only the hash of the sequence as computed by the function below would suffice.
<br><br>

<pre>def sequence_hash(sequence, B, M):
   result = 0
   for number in sequence:
       result = (result * B + number) % M

   return result
</pre>
<br><br>

<h3>Input</h3>
The first line contains an integer <strong>T</strong>, denoting the number of test cases. Each of the next subsequent <strong>T</strong> lines contain three positive integers, <strong>N</strong>, <strong>B</strong> and <strong>M</strong>.
<br><br>

<h3>Constraints</h3>
<strong><li>1 ¡Ü T ¡Ü 1000</li></strong>
<strong><li>2 ¡Ü N ¡Ü 10<sup>9</sup></li></strong>
<strong><li>N &lt; B ¡Ü 10<sup>9</sup></li></strong>
<strong><li>1 ¡Ü M ¡Ü 10<sup>9</sup></li></strong>

<h3>Output</h3>
For each test case, first print the case number followed by the minimum absolute difference and the hash of the lexicographically smallest partition <strong>P<sub>1</sub></strong>.

<h3>Sample Input</h3>
<pre>12
2 10 1000000000
3 10 1000000000
4 10 1000000000
5 10 1000000000
6 10 1000000000
7 10 1000000000
8 10 1000000000
9 10 1000000000
1000 1000000000 1000000
1000000 1003001 998244353
123456789 987654321 666666667
444444444 666666666 888888888

</pre>

<h3>Sample Output</h3>
<pre>Case 1: 1 1
Case 2: 0 12
Case 3: 0 14
Case 4: 1 124
Case 5: 1 1234
Case 6: 0 1247
Case 7: 0 12348
Case 8: 1 123457
Case 9: 0 1000
Case 10: 0 553178755
Case 11: 1 214459309
Case 12: 0 557434257
</pre>

<h3>Challenge</h3>
Don't like challenges? Try the easier version here:
<br><br>
<a href="https://www.spoj.com/problems/BPM/">Bipartite Permutation</a>