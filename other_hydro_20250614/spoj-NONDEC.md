<p>A Non-Decreasing number is a number whose ith digit from the left it greater than or equal to the (i-1)th digit from the left. <br> You are given four integers A, B, C and D. X is any  integer b/w A and B, inclusive, and Y is any integer b/w C and D,  inclusive. You must output the number of numbers formed by the  concatenation of X and Y which are Non-Decreasing, i.e. if we treat "X"  and "Y" as STRINGS, then "Z" = "X" + "Y" must represent a Non-Decreasing  number.  <br> Since this number can be very large, give your answer modulo 98765431. <br> If the same number "Z" can be formed in various ways, it must be counted every time. See example for clarification.</p>
<h3>Input</h3>
<p>The first line of the input contains t, the number of test cases. <br> This is followed by t lines containing 4 positive integers each, which are the values of A, B, C, D.</p>
<h3>Output</h3>
<p>You must output t lines. Each line contains the answers for the quadruple (A, B, C, D) in the order they appear in input.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>1<br>1 11 1 11
<strong>Output:</strong>
56<br><br><strong>Explanation</strong><br>Note that the number "111" is counted twice. Once as "11" + "1" and again as "1" + "11".<br><br></pre>
<h3>Constraints</h3>
<p>A, B, C, D are all positive integers having &lt;= 1000 digits <br> A &lt;= B; C &lt;= D; <br> Number of test cases = t &lt;= 1000</p>