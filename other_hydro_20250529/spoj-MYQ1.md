<p>
The seats of an Ultra Deluxe Semi-sleeper bus in Thuvax country are numbered according to the following rules:

</p><ol>
  <li>Seat number 1 is reserved for the bus conductor.</li>
  <li>Remaining seats are numbered as shown in the figure below.</li>
  <li>The seating arrangement is as shown below.
<pre>RowNo Left&nbsp;&nbsp; Right
      W&nbsp; A&nbsp;&nbsp; A&nbsp; M&nbsp; W
&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp; &nbsp; 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 01 
1&nbsp;&nbsp;&nbsp;&nbsp; 02 03&nbsp; 04 05 06
2&nbsp;&nbsp;&nbsp;&nbsp; 11 10&nbsp; 09 08 07
3&nbsp;&nbsp;&nbsp;&nbsp; 12 13&nbsp; 14 15 16
4&nbsp;&nbsp;&nbsp;&nbsp; 21 20&nbsp; 19 18 17
5&nbsp;&nbsp;&nbsp;&nbsp; 22 ............ &nbsp;  
   </pre></li>
</ol>

<p>A blind person enters the bus with a reservation ticket mentioning his seat number. He meets you at the start of the passage and&nbsp;shows you his ticket. Based on the seat number, help him find his seat by telling him the row number (1,2,...), seat position(window or aisle or middle), and the direction(left or right).</p>

<h3>Input</h3>
<p>First line contains a positive integer t (t &lt;= 10^5) denoting the number of test cases. </p>
<p>Each of the next t lines contain a positive integer n (n &lt;= 10^9) denoting the blind person's seat number.</p>

<h3>Output</h3>
<p>Output one line for every test case in the following format:
</p><ul>
  <li>If the seat number is same as the conductor's seat, print "<tt>poor conductor</tt>"</li>
  <li> else, print &lt;row_number&gt; &lt;seat_position&gt; &lt;direction&gt;
  <ul>
    <li>row_number: represents the row number from the entrance (a positive integer) &nbsp;</li>
    <li>seat_position: can be one of "W" or "A" or "M" for window, aisle and middle respectively. </li>
    <li>direction: can be either "L" or "R" for left or right respectively.</li>
  </ul>
  </li>
</ul>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
1
2
3

<strong>Output:</strong>
poor conductor
1 W L
1 A L</pre>