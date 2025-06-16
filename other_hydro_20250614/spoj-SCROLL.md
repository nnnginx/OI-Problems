<p>Sruthi is looking at a spreadsheet containing N rows. Only K rows of the spreadsheet are visible at a time (If the top row is i, the bottom row will be i+K-1). In the beginning, rows 1..K are visible. Sruthi needs to read certain values from rows r1,r2...rM in that order. It is possible to scroll the spreadsheet so that the rows j..j+K-1 can be viewed instead of the current i..i+K-1. This operation counts as one scroll and its scroll length is defined as |j-i|</p>
<p>Find the minimum number of scrolls required so that Sruthi can read of all the M values in the given order. As there may be more than one way to do this, also find the minimum total scroll length required to do the reading in so many scrolls.</p>
<h3>Input</h3>
<p>The first line of the input contains the integer T (&lt;=20), the number of test cases to follow.</p>
<p>The description of each test case begins with a line containing 3 integers N(&lt;=10^8), K(&lt;=10^8) and M(&lt;=50000) as defined in the problem. Following this are M lines giving the row numbers from which values have to be read sequentially.</p>
<h3>Output</h3>
<p>Output two space separated integers in a line per test case : The minimum number of scrolls required and the minimum scroll length required for the minimum number of scrolls.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
20 10 2
10
20
20 10 2
10
7

<strong>Output:</strong>
1 10
0 0
</pre>