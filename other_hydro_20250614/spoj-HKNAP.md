Our King has won the brutal battle and this whole land is now ours. The special thing about this land is that it has many beautiful golden statues. Our King wants to take back as much gold as possible to his palace. We have found that there are <strong>N</strong> types of statues
and -- almost unbelievably -- that there is an unlimited
number of each type of statue. Each statue of type <strong>i</strong> has a weight of <strong>W[i]</strong> units and occupies <strong>V[i]</strong> units of volume. Our King wants to maximize the amount of gold he
carries back to his palace. We may use <strong>S</strong> sacks for this purpose, each of volume <strong>Y</strong>.
All sacks are filled up independently by golden statues. However, there is a provision to stitch two sacks together, at the cost of <strong>C</strong>
units of gold. Stitching three sacks costs 2*C because it requires two stitchings, and so on. Your task is to find
how much gold our King can possibly gain, i.e. the
total weight of the statues brought back, minus the stitching charges.<p></p>
<h3>Input</h3>
<p>  T ¨C The number of test cases.<br>
  For each test case :<br>

  N S Y C // 1st line<br>
Next N lines two numbers W[i] and V[i] each.</p>
<h3>Output</h3>
<p>One integer, the maximum gain in gold for our King.<br>
  This gain is the total amount of gold transported minus stitching charges.</p>
<p><strong>Constraints :</strong><br>
  1&lt;= S &lt;= 1000 <br>

  1&lt;= Y &lt;= 1000 000 000<br>
  1&lt;= N &lt;= 1000<br>
  1&lt;= W[i] &lt;= 100; (for all i)<br>
  1&lt;= V[i] &lt;= 18; <br>

  The Output will fit into a 64-Bit integer. <br>
  1&lt;=T&lt;=20<br>
  All W[i] &amp; V[i] are guaranteed to be either prime or equal to 1.</p>
<h3>Example</h3>
<tt>
<p><strong>Sample Input:</strong><br>

  2<br>
  2 5 3 1<br>
  1 2<br>
  5 7<br>
  2 5 3 1<br>
  1 2<br>

  7 5<br>
  <br>
  <strong>Sample Output:</strong><br>
6<br>
17</p>
</tt>