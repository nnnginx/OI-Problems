<p>The new catchphrase of Jumbo Airlines is "No annoying neighbors, each flight a unique experience!"</p>
<p>And as in most cases, the advertisement was produced by the marketing department, without ever consulting the engineers. They only learned about it after the boss asked them to "handle it ASAP".</p>
<p>There are M seats in each row, and there are N rows of seats in the airplane. Hence the seats form an M * N grid. (For the purpose of this problem we will ignore the presence of aisles.) The airline sells exactly K tickets for each flight.</p>
<p>To make sure that the "no annoying neighbors" part of the motto is satisfied, the seating must obey the following rule: Whenever a seat is occupied, the seats immediately in front of it and behind it, as well as the seats immediately to the left and to the right must remain free.</p>
<p>An allowed arrangement is a set of K occupied seats that obeys the rule above.</p>
<p>The "unique experience" part of the motto is then satisfied by using a different arrangement of occupied seats for each flight. (Two seating arrangements are different if there is at least one seat which is occupied in one arrangement and free in the other.)</p>
<h3>Problem specification</h3>
<p>You are given the numbers M, N and K. Find the number of different allowed seating arrangements.</p>
<p>As this number can be very large, we're only interested in its value modulo 420047.</p>
<h3>Input specification</h3>
<p>Multiple test cases, seperated by blank lines.</p>
<p>Each test case consists of a single line containing three integers M, N and K. (M &lt;= N)</p>
<p>There are two kinds of input:</p>
<p>The input of the first kind satisfies that 1&lt;= M &lt;=15, 1&lt;= N &lt;=50, 3&lt;= K &lt;=50.</p>
<p>The input of the second kind satisfies that 1&lt;= M&lt;= 4, 1&lt;= N &lt;= 10<sup>9</sup>, 3&lt;= K &lt;=5.</p>
<p>Input terminates by EOF.</p>
<h3>Output specification</h3>
<p>For each test case output a single line with the number of allowed arrangements modulo 420047.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 4 4

<strong>Output:</strong>
2
</pre>
<h3>Hint</h3>
<p>The input file can be downloaded <a href="http://www.spoj.com/content/john_jones:airlines.in">here</a>. You may submit a TEXT file - the corresponding output file.</p>