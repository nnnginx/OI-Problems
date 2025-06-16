<p>Little Tulip recently learnt about how to &nbsp;write numbers. So she wrote some numbers in a paper in a line. But she never wrote a number which is less than the prevous one.</p>
<p>Now she want to know how many different numbers are in a given range.</p>
<p>In short, you are given an array of N integers indexed from 1 to N, and q queries, each in the form i j, you have to find the number of distinct integers from index i to j (inclusive).</p>

<h3>Input</h3>
<p>Input starts with an integer T (¡Ü 15), denoting the number of test cases.</p>
<p>The first line of a case is a blank line. The next line contains two integers N (1 ¡Ü N ¡Ü 10^5), q (1 ¡Ü q ¡Ü 10^5). The next line contains N space separated positive integers forming the array. Each of the next q lines will contain a query which is in the form i j (1 ¡Ü i ¡Ü j ¡Ü N).</p>

<h3>Output</h3>
<p>For each test case, print the case number in a single line. Then for each query you have to print a line containing number of distinct integers from index i to j.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2

5 3
1 2 2 4 5
1 2
1 5
4 5

3 1
1 1 1
1 3


<strong>Output:</strong>
Case 1:
2
4
2
Case 2:
1</pre>