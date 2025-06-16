<div align="justify">
<p>
Cool numbers are those, whose digits can be partitioned into two sets such that the sum of the digits in either sets are equal. <br>
Example: 23450 is cool because 3+4+0 = 2+5; So is 91125;<br>
The numbers 567, 34523 are not cool, since there is no such digit partition.<br>
<br>
Write a program that prints the number of cool numbers in the inclusive range [A,B].<br>
</p>
<br>
<b>Input Format:</b><br>
The input file consists of multiple testcases. <br>
Each case contains one line containing two 32-bit unsigned integers A and B. (1 &lt;= A &lt;= B &lt;= 4*10<sup>9</sup>).<br>
Input terminates with a line containing two zeros and must not be processed.<br>
<br>
<b>Output Format:</b><br>
For each testcase print a single line containing one integer saying the number of cool numbers between A and B, inclusive.<br>
<br>

<b>Sample Input:</b><br>
<pre>1 11
12 20
1 20
3 100
6354 234363
123456789 234567891
0 0
</pre>

<b>Sample Output:</b><br>
<pre>1
0
1
9
82340
54801678
</pre>
<br>
<b>Test Data:</b><br>
About 50 testcases.<br>
<br>
</div>