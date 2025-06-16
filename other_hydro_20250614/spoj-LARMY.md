<p><em>"A Lannister Always Pays His Debts."</em></p>
<p>That's true, now here is a chance for you to get paid by Jaime Lannister.</p>
<p>In Jaime's army there are total <strong>N</strong> number of warriors.</p>
<p>And all them are standing in a single row.</p>
<p>Now Jaime wants to convey a message to his warriors. But it's very difficult to convey a message if warriors are standing in a single row.</p>
<p>So, Jaime wants to break that single row into <strong>K</strong> rows. Such that in each row at least one warriors should be there.</p>
<p>Also, there is an amount of unhappiness associated with each warrior x which is equal to : number of warriors in front of x (in his row) whose height is greater than the height of x. And, total unhappiness is sum of unhappiness of all warriors. Jaime wants that his army should be happy as much as possible.</p>
<p>Now, Jaime wants you to break the single row into <strong>K</strong> rows such that total unhappiness should be minimum.</p>
<p><strong>Note</strong> : You just have to break the row, you are not allowed to change the position of the warriors.</p>
<p>&nbsp;</p>
<p><strong>Input Format</strong></p>
<p>First line of input contain two integers <strong>N</strong> &amp; <strong>K</strong>.</p>
<p>Second line of input contain <strong>N</strong> number of integers, <strong>i</strong> th of which denote height of <strong>i</strong> th warrior standing in that single row (represented as <strong>H[i]</strong>).</p>
<p>&nbsp;</p>
<p><strong>Constraints</strong></p>
<p>1 &lt;= <strong>N</strong> &lt;= 5000</p>
<p>1 &lt;= <strong>K</strong> &lt;= N</p>
<p>1 &lt;= <strong>H[i]</strong> &lt;= 10^5</p>
<p>&nbsp;</p>
<p><strong>Output Format</strong></p>
<p>Output the minimum possible value of "total unhappiness".</p>
<p>&nbsp;</p>
<p><strong>Examples</strong>&nbsp;</p>
<p><strong>Input</strong></p>
<p>6 3</p>
<p>20 50 30 60 40 100</p>
<p><strong>Output</strong></p>
<p>0</p>
<p><strong>Explanation</strong></p>
<p>Break as :</p>
<p>Row 1 : 20 50</p>
<p>Row 2 : 30 60</p>
<p>Row 3 : 40 100</p>
<p><strong>Input</strong></p>
<p>8 3</p>
<p>20 50 30 60 40 100 5 1</p>
<p><strong>Output</strong></p>
<p>2</p>
<p><strong>Explanation</strong></p>
<p>Row 1 : 20 50 30 60, Unhappiness = 1</p>
<p>Row 2 : 40 100, Unhappiness = 0</p>
<p>Row 3 : 5 1, Unhappiness = 1</p>
<p>Total = 2<br><br><strong>Update : Time limit increased.</strong></p>