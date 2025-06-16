<p>According to Wikipedia, a Walsh matrix is a specific square matrix, with dimensions equal to a power of 2, the entries of which are +1 or -1, and the property that the dot product of any two distinct rows (or columns) is zero. Below are the first three Walsh Matrices. (The gray lines are imaginary lines for illustration purpose only.)
</p><p style="text-align: center;">
<img src="./21372/file/wr3bQWwa.png">
</p><p style="text-align: left;">
A Walsh Matrix of size 2^(N+1)  can be constructed as the "union" of 4 Walsh Matrices of size 2^N  arranged such that the lower right matrix is inverted whereas the other 3 matrices are not, i.e.:
</p><p style="text-align: center;">
<img src="./21372/file/7TXyv5Tb.png">
</p><p style="text-align: left;">
Let's number the rows of a given Walsh Matrix from the top starting with row 0. Similarly, let's number the columns of the matrix from the left starting with column 0. Given the four integers N , R , S , and E , write a program that will construct a Walsh Matrix of size 2^N  and will print the sum of all the numbers in row #R between columns #S and #E (inclusive.)
</p><h3>Input</h3>
<p>Your program will be tested on one or more test cases. Each test case is specified using a single line listing four integers in the following order: N , R , S , and E , where 0 &lt;= N &lt;= 60 , 0 &lt;= R &lt; 2^N  , 0 &lt;= S &lt;= E &lt; 2N  , and E - S &lt;= 10,000 . The last line of the input file has four -1's and is not part of the test cases.

</p><h3>Output</h3>
<p>For each test case, print the output on a single line.

</p><h3>Example</h3>

<pre><b>Input:</b>
2 1 0 1
48 0 0 47
-1 -1 -1 -1

<b>Output:</b>
0
48
</pre>