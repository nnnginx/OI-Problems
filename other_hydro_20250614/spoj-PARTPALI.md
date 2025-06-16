<p>A palindromic decimal integer reads the same forward and backward.
For example, the following numbers are palindromic.</p>

<p>6, 55, 282, 5005, 78187, 904409, 3160613, 11111111</p>

<p>Palindromic integers are plentiful. In fact, any integer not
divisible by 10 has an infinite number of multiples that are
palindromic. (The standard representation of a nonzero multiple of 10
cannot be palindromic since its reversal would have a leading 0.)</p>

<p>Write a program to determine, for a given positive integer, how
many of its positive multiples are palindromes of a given length.</p> 



<h3>Input</h3>

<p>
The first line of the input will specify an integer n indicating the
number of problem instances to follow, one to a line.  Each of the
ensuing  n  lines will specify a pair of positive integers   m,s
separated by a single space, with 
1 &lt;  m  &lt; 1000,  s &lt; 20.    (For m,s in this range, there are
fewer than 2^32 palindromes among the s-digit multiples of m.)  Each
line will terminate with an end-of-line.</p>


<h3>Output</h3>

<p>The output should indicate  for each m,s, exactly how many s-digit
positive palindromes are divisible by m, with one problem instance per
line.   </p> 


<h3>Example</h3>

<pre><b>Input:</b>
5	
3 1	
25 3	
12 4	
30 3
81 6


<b>Output:</b>
3
2
7
0
0

</pre>

<p><b>Explanation:</b> There are three positive 1-digit multiples of
3, namely, 3, 6, and 9; all 1-digit numbers are trivially palindromes.
Among the 3-digit palindromes, 525 and 575 are multiples of 25.  The
4-digit multiples of 12 that are palindromes are 2112, 2772, 4224,
4884, 6336, 6996, 8448.   There are no positive palindromic numbers
ending in 0 (since we do not allow leading 0's).  No 6-digit
palindromes are divisible by 81.</p>