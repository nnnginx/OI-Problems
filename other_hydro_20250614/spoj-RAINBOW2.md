<p>This time Blue Mary continues doing meaningless calculations! (see problem <a href="http://www.spoj.com/problems/SPY2">SPY</a>) She is interested in calculating the <b>K</b>-th power of a very large <b>N</b>x<b>N</b> matrix A, where</p>
<p>A<sub>i,j</sub> = i * <b>D</b> + <b>Q</b><sup>j</sup> </p> 
<p>i and j are 0-based index of the row and column of element A<sub>i,j</sub>, respectively.
</p><p>Now she needs your help (again).</p>
<p>To keep the output small, you are only asked to output some of its elements.</p>
<h3>Input</h3>
<p>Multiple test cases.</p>
<p>The first line of each test case contains 5 space-separated integers <b>N</b>, <b>K</b>, <b>D</b>, <b>Q</b>, <b>M</b> in this order. <b>M</b> lines follow, each contains two space-separated integers <b>R<sub>i</sub></b> and <b>C<sub>i</sub></b>. </p>
<p>Input terminates by EOF.</p>
<p>All input numbers are non-negative integers and no more than 10<sup>9</sup>.(<b>D</b>, <b>R<sub>i</sub></b> and <b>C<sub>i</sub></b> may be 0, others must be positive integers.) <b>N</b> and <b>M</b> will be no more than 10<sup>5</sup>. <b>R<sub>i</sub></b> and <b>C<sub>i</sub></b> will be less than <b>N</b>. </p> 
<p>Input is almost uniformly-random generated, and the number of "large" test cases is relatively small.</p>
<h3>Output</h3>
<p>For each test case output exactly <b>M</b> lines. Each line contains only one integer: The number at the <b>R<sub>i</sub></b>-th row and <b>C<sub>i</sub></b>-th column (0-based) of the matrix <b>A<sup>K</sup></b>. As the result may be quite large, output it modulo 10<sup>9</sup>+2015. </p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 3 0 1 10
0 0
1 1
2 2
3 3
4 4
5 5
6 6
7 7
8 8
9 9
2 2 1 2 4
0 0
0 1
1 0
1 1

<strong>Output:</strong>
100
100
100
100
100
100
100
100
100
100
5
8
8
13
</pre>