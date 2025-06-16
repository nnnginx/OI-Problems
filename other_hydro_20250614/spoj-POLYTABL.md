<p>Given a polynomial, your task is to print a table of some of its calculated values.</p>
<h3>Input</h3>
<p>Input starts with a positive integer t&lt;1000, the number of testcases, then t testcases follow. Every testcase contains the representation of a polynomial of at most fourth degree in "pretty printing" notation. Coefficients  are either given as integers or fractions. The absolute values of all numbers including numerator and denominator are not larger than 100.</p>
<p>If all coefficients are integers and degree is not larger than 1, a polynomial (which means a testcase) is given in a single line (the <em>base line</em>).<br> If all coefficients are integers, but degree is larger than 1, a polynomial is given in two lines. The first of these contains only the exponents, the second  line is the <em>base line</em>.<br> If at least one coefficient is given as a fraction, a polynomial is given in three lines. The first line contains the exponents (if there are any) and the numerators, the last line the denominators.</p>
<p>Polynomials are given in <strong>canonical form</strong>, which means:<br> ⇢ powers of x are given in decreasing order and do not appear more than once<br> ⇢ there is always exactly one operator (either + or -) between consecutive summands<br> ⇢ coefficients with an absolute value of 1 are left out<br> ⇢ summands with coefficients with a value of 0 are left out except for the null polynomial<br> ⇢ there are no whitespaces in the base line except those below exponents</p>
<p>The fraction bar is formed by as many dashes as there are digits in numerator respectively denominator. If the number of digits in numerator and denominator is different, the fraction bar is as long as the larger value; the smaller one is aligned to the right.</p>
<pre style="color:green; font-weight:bold">                          3 4  2                3  10        2
Valid polynomials are:   --x +x     -x+2      5x +---       x -5
                          5                       100
</pre>
<pre style="color:red; font-weight:bold">                         -3 4  2        2           1                    3
Invalid polynomials are:  -x +x        x+3x      x---      4x -13      2x +-5
                          5                         7
</pre>
<p>The base line of the polynomial is followed by a single space, then the information about the range of calculation is given.  It is denoted as "[a;b;m]", where a,b and m are integer values with -10 ≤ a &lt; b ≤ 10 and 1 ≤ m ≤ 50.  You have to divide [a;b] into m equal width sections of width d and calculate the polynomial's values for x=a, x=a+d, x=a+2d, …, x=b.</p>
<p><em>Note: There are no trailing whitespaces and every testcase is followed by a blank line.</em></p>
<h3>Output</h3>
<p>For every testcase print a table with the polynomial's values as shown in the example below. The output for every testcase consists of nine lines. The first and the last line  are an identical sequence of dashes. All other lines start and end with "|", columns are also separated by "|" resp. "+" in the fifth line that separates the rows.   The leftmost column contains x in the top row and the polynomial (exactly as given in the input) in the bottom row.  The other columns are filled with the x-values in the top row in increasing order and the corresponding y-values in the bottom row. The width of a column depends on the maximum width of the values inside (may be  in the top or bottom row) plus an additional space to the left and to the right.  If the corresponding value in the other row needs less space, it is aligned to the right.</p>
<p>Regardless of the type of value – integer or fraction – the rows are always three lines in height. Integer values, fraction bars and signs are always printed in the middle line, numerator and denominator one line above resp. below. Fractions must be printed in lowest terms. If the value of a fraction is an integer value, it has to be printed as integer.  No (intermediate) value will have an absolute value larger than 10¹⁸, if calculations are done carefully. The width of the fraction bar and alignment of numerator resp. denominator follow the same rules as explained in the input section.  <em>Print a blank line after every testcase except the last one.</em></p>
<p style="font-weight:bold; color:#880000">Note: The "exact judge" is used here, so the output format must be precisely observed.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
 3   2
x -4x  [-2;3;5]

 3 2   3
--x +x+- [-1;4;10]
 8     8


<strong>Output:</strong>
----------------------------------------
|        |     |    |   |    |    |    |
|      x |  -2 | -1 | 0 |  1 |  2 |  3 |
|        |     |    |   |    |    |    |
|--------+-----+----+---+----+----+----|
|  3   2 |     |    |   |    |    |    |
| x -4x  | -24 | -5 | 0 | -3 | -8 | -9 |
|        |     |    |   |    |    |    |
----------------------------------------

------------------------------------------------------------------
|          |    |   1 |   |  1 |   |  3 |   |  5 |   |   7 |     |
|        x | -1 |  -- | 0 |  - | 1 |  - | 2 |  - | 3 |   - |   4 |
|          |    |   2 |   |  2 |   |  2 |   |  2 |   |   2 |     |
|----------+----+-----+---+----+---+----+---+----+---+-----+-----|
|  3 2   3 |    |   7 | 3 | 25 |   | 33 | 7 | 17 |   |  23 |  13 |
| --x +x+- | -1 | --- | - | -- | 1 | -- | - | -- | 0 | --- | --- |
|  8     8 |    |  32 | 8 | 32 |   | 32 | 8 | 32 |   |  32 |   8 |
------------------------------------------------------------------
</pre>