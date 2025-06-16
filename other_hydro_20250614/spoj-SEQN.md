<p>As you know, there number of permutation of the increasing vector {1, 2, 3¡­n} is exactly n! ;For example, if n = 3, then, {1,2,3} , {1,3,2}, {2,1,3}, {2,3,1}, {3,1,2}, {3,2,1} are all the permutation of the vector {1,2,3 };</p>
<p><strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; We define D( {</strong>A1,A2...An <strong>} ) = the number of element that satisfy&nbsp;&nbsp; Ai = i.<br></strong></p>
<p><strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>For example, D( {1,2,3} ) = 3 ,D( {1,3,2} ) = 1 (only ¡®1¡¯ is at 1), D({3,1,2}) = 0 ¡­.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Now we want to calculate the number of permutation that satisfy D( {A1,A2...An   } ) = K.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; For example, if n = 3 and k = 3, then of course there is only one permutation {1,2,3} that satisfy D( {1,2,3}) = 3. But if n = 3 and k = 0, then there are two permutations {3,1,2} and {2,3,1} satisfy D( {3,2,1} ) = D( {2,3,1} ) = 0;</p>
<p>&nbsp; But when n is very large, it¡¯s hard to calculate by brute force algorithm. Optimal is one required here.</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Because the answer may be very large, so just output the remainder of the answer after divided by m.</p>

<h3>Input</h3>
<p>In the first line there is an integer T, indicates the number of test cases. (T &lt;= 500)</p>
<p>In each case, the first line contains three integers n,k and m. (0 &lt;= k&lt;= n &lt;=10^9, 1 &lt;= m &lt;= 10^5, n != 0)</p>

<h3>Output</h3>
<p>Output ¡°Case d: ¡°first where d is the case number counted from one. Then output the remainder of the answer after divided by m.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>3 0 7<br>3 3 3<br>331105236 82934100 3711<br><br><br><strong>Output:</strong><br>Case 1: 2<br>Case 2: 1<br>Case 3: 2622</pre>