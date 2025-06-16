<p>As the winner of the competition, you are asked to take prizes that are numbered from 1 to K. Each i-prize weighs Wi kg and is worth Hi dollar. You are carrying a bag with a capacity of N kg. The gifts must be put in this bag to be taken home. Each prize must be taken in its entirety and may not be taken in certain parts. Determine which gifts need to be brought, so that the total value of the gifts brought can be as maximum as possible. You may carry a number of gifts, so that the total weight is still &lt;= N kg.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains the testcase T (1 &lt;= T &lt;= 100), as many as T the next line contains two integers separated by spaces, namely N and K.</p>
<p>The next K line contains two Wi and Hi numbers, which represent a description of a gift.</p>
<h3>Output</h3>
<p>Print the serial number of the prizes so that the total value is maximum. Print these numbers in order from small to large.</p>
<p>If there is more than one optimal stone picking method, print out a method for picking stones that minimizes weight.</p>
<p>If there is more than one method, prioritize the stones with the smaller number.</p>
<p>&nbsp;</p>
<p><strong>Constraint :</strong></p>
<p>1 ¡Ü N ¡Ü 2,000</p>
<p>1 ¡Ü K ¡Ü 100</p>
<p>1 ¡Ü Wi, Hi ¡Ü 2,000, for 1 ¡Ü i ¡Ü K</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>5 3
9 3
10 2
32 2</pre>
<pre>11 3
10 30
6 17
5 14

<strong>Output:</strong>
Case 1:
0
Case 2:
2
3</pre>