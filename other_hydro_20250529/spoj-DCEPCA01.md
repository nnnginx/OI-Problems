<p>A number is called lucky if it consists of only digits 4 and 7 ie. 4, 7, 44, 47 are lucky numbers while 3, 45, 4478 are not lucky. For a given lucky number the functions F(i) and G(i) are defined as follows</p>
<p>F(i) = the number of 4¡¯s from 0<sup>th</sup> to i<sup>th</sup> position in the number including positions 0 and i.<br>G(i) = the number of 7¡¯s from 0<sup>th</sup> to i<sup>th</sup> position in the number including positions 0 and i.</p>
<p>Let H(i)= absolute(F(i)-F(i+1)-F(i+2)+F(i+3))</p>
<p>A "Dynamic Number" is a lucky number which has maximum of summation(H(i)) from i = 0 to n-4 amongst all lucky numbers of length N.</p>
<p>Given a number N , you need to find out the sum of the two smallest Dynamic Numbers of length N.If only one Dynamic Number is possible, then only that number is the answer.</p>
<p>Note : Most significant bit is defined as the 0<sup>th</sup> position of the number.</p>
<h3>Constraints</h3>
<p>0 &lt; T &lt;= 100<br>4 &lt;= N &lt;= 10^5</p>
<h3>Input</h3>
<p>It consists of T+1 lines. T denotes the number of test cases. Followed by T lines, each containing one number N.</p>
<h3>Output</h3>
<p>Output T lines, each containing a number as required.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1<br>4<br><br><strong>Output:</strong>
8924</pre>