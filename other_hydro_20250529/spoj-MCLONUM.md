<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MCLONUM/en/">English</a></td> 
<td width="50%"><a href="/problems/MCLONUM/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<pre>Consider  two n-digit positive decimal  integers A and B with no  leading
zeroes. We need  to  find  the two closest to A n-digit numbers (the 
first one �C greater or equal to A, the other �C strictly less than A), 
with decimal writings containing all the digits of B in some order.  
For example  if A=3022  and B=1232, using B��s digits we can obtain  
the  following 4-digit numbers: 1223,  1232,  1322,  2123,  2132,  2213,
2231,  2312,  2321,  3122,  3212  and  3221.  The  least  number greater 
or equal to A obtained by B��s digits is 3122, and the biggest one, 
strictly less then A is 2321. If A=1232 and B=3022, the possible numbers
are 2023, 2032, 2203, 2230, 2302, 2320, 3022, 3202 and 
3220. The  least number greater or equal  to A obtained by B��s digits
is 2023, and  there  is no number less than A. 
Write a program closest  to find  these ��closest  to A�� numbers for
given A and B, or  to determine that one of them does not exist.</pre>
<h3>INPUT </h3>
<pre>Two lines are read from the standard input, each of them containing an
n-digit positive integer with no leading zeroes, with A read from the
first, and B read from the second line (1��n �� 60).</pre>

<pre>SAMPLE INPUT
Example 1        Example 2
3075             3000203 
6604             4562454</pre>

<h3>OUTPUT  </h3>
<pre>Write to the standard output: 
-  Line  1:  the  least  n-digit  number with  no  leading  zeroes,
not  less  than  A,  containing  all  the digits of B in some order. 
If such number does not exist, the output should be 0. 
-  Line 2: the biggest n-digit number with no leading zeroes, less
than A, containing all the digits of B in some order. If such number 
does not exist, the output should be 0.
SAMPLE OUTPUT
Example 1      Example 2
4066           4244556 
0              2655444 
</pre>
<b>Problem for kid - Please, think like kid.</b>