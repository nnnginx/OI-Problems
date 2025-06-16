<!-- 		@page { margin: 0.79in } 		P { margin-bottom: 0.08in } -->
<p style="margin-bottom: 0in" align="JUSTIFY">Ashton Carl McDonalds (known as A.C.M.) works at a company called XOR (XptO Revolution). The company has a simple rule for employee identification: each employee must have an integer id that must be unique (no two employees may have the same id).</p>
<p style="text-indent: 0.49in; margin-bottom: 0in" align="JUSTIFY">Recently, the employees were grouped into teams, in the following way: the teams are intervals on the XOR¡¯s employees list. An employee can be part of more than one team.</p>
<p style="text-indent: 0.49in; margin-bottom: 0in" align="JUSTIFY">The company wants to hire new employees, and needs to generate id numbers for them. However, due to a security flaw in Human Resources software, the company can¡¯t assign a new number that, if one executes Exclusive-Or operation with all numbers of any team, results in 0.</p>
<p style="text-indent: 0.49in; margin-bottom: 0in" align="JUSTIFY">McDonalds, as the leader lazy programmer of XOR, needs your help to determine if a given number can or can¡¯t be assigned to a new employee.</p>
<h3>Input</h3>
<!-- 		@page { margin: 0.79in } 		P { margin-bottom: 0.08in } -->
<p>The input contains multiple test cases.</p>
<p style="margin-bottom: 0in" align="JUSTIFY">The first line of each test case contains three numbers, N, T and Q, the number of employees in the company, the number of teams and the number of new numbers to be queried, respectively.</p>
<p style="margin-bottom: 0in" align="JUSTIFY">The second line contains N numbers X<sub>i</sub>, 1 &lt;= i &lt;= N, distinct, the employees id numbers.</p>
<p style="margin-bottom: 0in" align="JUSTIFY">Each one of the following E lines contains two numbers, A and B, which represent an interval that forms a team. It means that the employees identified by X<sub>A</sub>, ¡­,  X<sub>B</sub> form one team.</p>
<p style="margin-bottom: 0in" align="JUSTIFY">Each one of the following Q lines contains one number Y<sub>j</sub>, the queried number.</p>
<p style="margin-bottom: 0in" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in" align="JUSTIFY">Limits: 1 &lt;= N, T, Q &lt;= 10<sup>5</sup>, 1 &lt;= A &lt;= B &lt;= N. All X<sub>i</sub> and Y<sub>j</sub> will be non-negative and fit into a signed 32 bit integer, and all queries must be treated as independent from others (just the initial employees and teams must be taken into account).</p>
<h3>Output</h3>
<!-- 		@page { margin: 0.79in } 		P { margin-bottom: 0.08in } -->
<p style="text-indent: 0.49in; margin-bottom: 0in" align="JUSTIFY">For each test case, the program must print Q + 1 output lines. For each queried number, the program must print ¡®Y¡¯, if the number can be assigned to a new employee, or ¡®N¡¯, otherwise. The last line is a simple minus sign ¡®-¡¯.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<!-- 		@page { margin: 0.79in } 		P { margin-bottom: 0.08in } -->3 2 4<br>1 2 4<br>1 2<br>1 3<br>3<br>5<br>6<br>7<br>0 0 0

<strong>Output:</strong>
N<br>Y<br>Y<br>N<br>-
</pre>