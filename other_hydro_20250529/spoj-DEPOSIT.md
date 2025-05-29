<p>Banks offer deposit schemes of various kinds to attract customers. In an r -year progressively reducing recurring deposit scheme (PRRDS) of a bank, a customer is required to deposit progressively reducing amounts every year for r  years. Depending on the duration r  of the scheme and the total amount T  deposited in r  years, the bank offers to return on maturity, i.e., after the expiry of r  years, an amount R , which is equal to k  times the amount deposited in the first year. The bank ensures that the return R  looks attractive by making a suitable choice of k ; k  being a natural number.
</p>
<p>
In a PRRDS, the amount to be deposited in each but the last two years is exactly equal to the sum of amounts to be deposited in the next two years. The amounts to be deposited in the last two years, say x in the last year and y in the last but one year, are progressively reducing (x, y &gt; 0;y &gt; x) and are determined so that the total amount deposited in r years is exactly equal to the specified amount T . Assume that all deposits are in whole number of Rupees.
</p>
<p>
Write a program for the bank, so that given r , k and T , the program computes x and y for which the return R is maximum. For example in a 4-year scheme with r = 4 , k = 3 and T = 500 , the progressively reducing recurring deposits 248, 126, 122 and 4, ensures the maximum return R = 744 with x = 4 and y = 122 .
</p>
<h3>Input</h3>
<p>The input may contain multiple test cases.</p>
<p>For each test case there is only one input line. The line gives values of r , k and T . Assume that r is not greater than 20.</p>
<p>A line containing a zero `0' as the first character follows the last case.</p>

<h3>Output</h3>
<p>For each test case there is only one output line. The line gives the computed values of x , y and R .</p>

<h3>Example</h3>
<pre><b>Input</b>
4 3 500 
5 3 10000 
6 4 8000 
8 5 12000 
0

<b>Output</b>
4 122 744 
5 1425 12855 
1 666 13332 
1 363 23635
</pre>