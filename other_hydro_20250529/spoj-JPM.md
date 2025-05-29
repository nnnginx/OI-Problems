This problem is really simple, or is it? Given a positive integer <strong>N</strong>, calculate the <strong>minimum</strong> number of <strong>distinct</strong> primes needed such that their sum equals to  <strong>N</strong>. A prime number is a natural number greater than <strong>1</strong> that cannot be formed by multiplying two smaller natural numbers. The first few prime numbers are <strong>2, 3, 5, 7, 11, 13, 17, 19, 23, 29, ...</strong> and so on.
<br><br>

<h3>Input</h3>
The first line contains an integer <strong>T</strong>, denoting the number of test cases. Each of the next subsequent <strong>T</strong> lines contain a positive integer <strong>N</strong>.

<br><br>

<h3>Constraints</h3>
<strong><li>1 ¡Ü T ¡Ü 50,000</li></strong>
<strong><li>1 ¡Ü N ¡Ü 50,000</li></strong>

<h3>Output</h3>
For each test case, first print the case number followed by the minimum number of distinct primes such that their sum equals to <strong>N</strong>. If <strong>N</strong> cannot be represented by a summation of distinct primes, then print the case number followed by <strong>-1</strong>. Refer to the sample input/output for more clarity of the format.

<h3>Sample Input</h3>
<pre>10
1
2
3
10
27
100
1000
4572
4991
49999

</pre>

<h3>Sample Output</h3>
<pre>Case 1: -1
Case 2: 1
Case 3: 1
Case 4: 2
Case 5: 3
Case 6: 2
Case 7: 2
Case 8: 2
Case 9: 3
Case 10: 1
</pre>

<h3>Challenge</h3>
Too easy? Try the harder version here -  <a href="https://www.spoj.com/problems/JPM2/">Just Primes II</a>
<br><br>