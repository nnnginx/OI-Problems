<p>Given a positive integer <strong>N</strong>, calculate the minimum number of distinct primes required such that their sum equals to <strong>N</strong>. Also calculate the number of different ways to select these primes. Two ways are considered to be different <strong>iff</strong> there exists at least one prime in one set not existing in the other.</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>T</strong>, denoting the number of test cases. Each of the next subsequent <strong>T</strong> lines contain a positive integer <strong>N</strong>.</p>
<h3>Constraints</h3>
<p>&nbsp;</p>
<ul>
<li><strong>1 ¡Ü T ¡Ü 500,000</strong></li>
</ul>
<ul>
<li><strong>1 ¡Ü N ¡Ü 500,000</strong></li>
</ul>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, output two integers <strong>X</strong> and <strong>Y</strong> separated by a single space. <strong>X</strong> denotes the minimum number of distinct primes required such that their summation equals to <strong>N</strong>, and <strong>Y</strong> is the number of ways to select these primes. If it is not possible to express <strong>N</strong> as a summation of distinct primes, set <strong>X</strong> and <strong>Y</strong> to <strong>-1</strong> and output them. You can safely assume that the answer will always fit in a signed 32 bit integer.</p>
<h3>Sample Input</h3>
<pre>20
1
2
10
27
100
666
1000
1729
4572
4991
10000
100000
480480
482790
499799
499847
499901
499979
499999
500000
</pre>
<h3>Sample Output</h3>
<pre>-1 -1
1 1
2 1
3 3
2 6
2 31
2 28
3 2393
2 110
3 13396
2 127
2 810
2 8499
2 8291
3 31121027
3 31139901
3 31124665
1 1
3 30974053
2 3052
</pre>

<h3>Warm Up</h3>
Too hard? Try the easier version here -  <a href="https://www.spoj.com/problems/JPM/">Just Primes</a>
<br><br>