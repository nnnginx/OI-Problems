<div>
<div id="problem-statement-preview">
<p>Alia  has been assigned a homework by her maths teacher to find the  "Handsome" numbers. She is confused about these numbers, as we all know  that she is very "intelligent" :P</p>
<p>So she needs your help. Following is an exact line that her teacher  has given about Handsome numbers : "Handsome number can be defined as a number such that sum of all the  proper divisors of handsome number with modulus to m, has to be a devil  number.  This Devil number is a number whose total number of proper divisors , is  a Fibonacci number (0,1,1,2,3,5....)."</p>
<p>Note : Alia's lucky number is 1, so she assumes 1 as a proper divisor always :P</p>
<p><strong>Input Format :</strong></p>
<p>First line of input is t (no. of test cases) then next each t lines will contain two integers n (no. that is to be checked), m.</p>
<p><strong>Output Format :</strong></p>
<p>Print in a each output line Case no. and "YES." if a number is a handsome number otherwise "NO.". (with a dot)</p>
<pre><code>        Case_#i_:_YES.
        Case_#j_:_NO.
</code></pre>
<p>Here, '_' refers to a single space.</p>
<p><strong>Constraints :</strong></p>
<p>t &lt;= 100</p>
<p>2 &lt;= n &lt;= 10^9</p>
<p>1 &lt;= m &lt;= 10^8</p>
<p><strong>Sample Input :</strong></p>
<p>2</p>
<p>6 5</p>
<p>100 45</p>
<p><strong>Sample Output :</strong></p>
<p>Case #1 : YES.</p>
<p>Case #2 : YES.</p>
<p><strong>Explanation :</strong></p>
<p>Case #1 : proper divisors of 6 are 1, 2, 3 i.e sum = 6 , taking mod  with 5, i.e 1. Now no. of proper divisors of 1 is a Fibonacci number.</p>
</div>
</div>