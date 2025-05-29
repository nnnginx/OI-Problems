<p>You are given an matrix M (consisting of nonnegative integers) and an integer K. &nbsp;For any submatrix of M' of M define min(M') to be the minimum value of all the entries of M'. &nbsp;Now your task is simple: &nbsp;find the maximum value of min(M') where M' is a submatrix of M of area at least K (where the area of a submatrix is equal to the number of rows times the number of columns it has).</p>
<h3>Input</h3>
<p>The first line contains a single integer T (T ¡Ü 10) denoting the number of test cases, T test cases follow. &nbsp;Each test case starts with a line containing three integers, R (R ¡Ü 1000), C (C ¡Ü 1000)&nbsp;and K (K ¡Ü R * C)&nbsp;which represent the number of rows, columns of the matrix and the parameter K. &nbsp;Then follow R lines each containing C nonnegative integers, representing the elements of the matrix M. &nbsp;Each element of M is ¡Ü 10^9</p>
<h3>Output</h3>
<p>For each test case output two integers: &nbsp;the maximum value of min(M'), where M' is a submatrix of M of area at least K, and the maximum area of a submatrix which attains the maximum value of min(M'). &nbsp;Output a single space between the two integers.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
2 2 2
1 1
1 1
3 3 2
1 2 3
4 5 6
7 8 9

<strong>Output:</strong>
1 4
8 2</pre>