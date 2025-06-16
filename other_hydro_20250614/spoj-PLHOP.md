<p>This man has grown so rich that, when he travels between any
two locations he always takes atleast K flights. In a region of N
cities, we need to find the minimal cost required for the man to travel
between every pair of cities. There are provisions (especially for this
type of rich men,) to fly from i-th city to the i-th city itself!</p>
<h3>Input</h3>
<p>
  T ¨C The number of test cases. <br>
  In each test case :<br>
  K N<br>
NxN matrix representing the costs of the tickets. The i-th line, j-th
column¡¯s entry represents the cost of a ticket from city i to city j.
The numbers are of course space separated.</p>

<p><strong>Constraints :</strong><br>
  T&lt;=20<br>
  N&lt;=50<br>
  K&lt;=10<sup>9</sup><br>
  The cost of each ticket &lt;= 100<br>

  Each element of the output matrix will fit into a 
  64-bit integer.<br>
  </p>
<h3>Output</h3>
<p>For the i-th test case , 1st line is of the form ¡°Region #i:¡±. <br>
In the following N lines, output an NxN matrix where the j-th element
of the i-th line represents the minimal cost to travel from city i to
city j with taking atleast K flights. The numbers on a line must be
separated by atleast one space. Output a blank line after each testcase
(including the last one).</p>
<h3>Example</h3>
<tt>
<p><strong>Sample Input:</strong><br>
  2<br>

  3 4<br>
  1 2 3 4<br>
  5 6 7 8<br>
  9 10 11 12<br>
  13 14 15 16<br>
  10999 4<br>

  1 2 3 4<br>
  5 6 7 8<br>
  9 10 11 12<br>
  13 14 15 16</p>
<p><strong>Sample Output:</strong><br>
  Region #1:<br>

  3 4 5 6<br>
  7 8 9 10<br>
  11 12 13 14<br>
  15 16 17 18</p>
<p>Region #2:<br>
  10999 11000 11001 11002<br>

  11003 11004 11005 11006<br>
  11007 11008 11009 11010<br>
  11011 11012 11013 11014</p>
</tt>