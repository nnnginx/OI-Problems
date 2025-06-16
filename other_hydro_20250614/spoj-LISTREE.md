<p>You are given a tree with <strong>N</strong> vertices. Every vertex has an unique number from the interval<strong> [1, N]</strong>. Consider all simple paths on this tree. For every simple path you can write the sequence of numbers taken from consecutive vertices on this path. For every such sequence you can find the <a href="https://en.wikipedia.org/wiki/Longest_increasing_subsequence">Longest Increasing Subsequence</a>. Find the longest of all Longest Increasing Subsequences and print its length.</p>
<h3>Input</h3>
<p><em>The size of each input file is not greater than 2 MB.<br></em></p>
<p>In the first line of the input there is an interger <strong>T (1 ¡Ü T ¡Ü 1000)</strong> - the number of data sets.</p>
<p>In the first line of each data set there is an interger <strong>N (1 ¡Ü N ¡Ü 10<sup>5</sup>)</strong>.</p>
<p>In each of the next <strong>N - 1</strong> lines of the data set you can find two intergers <strong>a</strong> and <strong>b (1 ¡Ü a, b ¡Ü N) </strong>meaning that there is an edge connecting vertex with number <strong>a</strong> and vertex with number <strong>b</strong>.</p>
<h3>Output</h3>
<p>For each data set print one number: the length of the longest LIS of all simple paths.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
12
3 1
1 4
4 12
12 8
4 5
5 11
5 6
5 2
3 9
9 10
9 7
12
1 8
8 6
8 3
3 12
3 10
3 5
5 4
5 2
1 9
9 11
9 7
<strong>Output:</strong>
4
5
<strong>One of the solutions for the second tree in the example:</strong>
<strong><img src="file://kCO48iwX.png" alt="" width="622" height="508"></strong>
<div><strong><br></strong></div></pre>