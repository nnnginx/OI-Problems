<p>n persons are standing in a line. Height of each person is between 1 and n and height of each person is distinct.&nbsp;</p>
<p>You a given array A where A[i] denotes how many persons are before i_th person having heights greater than H[i]. eg. For person 2, person 1 is considered before him. If A is given to be [0, 1] then one valid arrangements of height could be [2, 1] as number of persons having height &gt; 1 before 2 are 1 because H[1] &gt; H[2]</p>
<p>You have to find out whether this array can be valid for some arrangement of persons. If you can uniquely do so, then find out the array H. Otherwise output -1.</p>
<h3>Input</h3>
<p>First line contains T : number of test cases. (1 &lt;= T &lt;= 20).</p>
<p>For each test First line contains an integer n. ( 1 &lt;= n &lt;= 10^5)</p>
<p>Next line contains n space seperated integers denoting A[i]. (0 &lt;= A[i] &lt;= n)</p>
<h3>Output</h3>
<p>For each test case output single line&nbsp;</p>
<p>If there is a unique way of H. Then print n space seprated integers in the line.</p>
<p>Otherwise output -1.</p>
<p>In starting of each test case also put "Test : testNumber" (without quotes). Note that there is a space before colon and one space after colon.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>3<br>0 1 1<br>3<br>0 1 0&nbsp;</pre>
<pre><strong>Output:</strong>
Test : 1<br>3 1 2<br>Test : 2<br>2 1 3</pre>