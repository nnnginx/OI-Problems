<p>N persons are standing in a line. Height of each person is between 1 and N and height of each person is distinct.&nbsp;</p>
<p>You are &nbsp;given an array A where A[i] denotes how many persons are there before the i_th person having heights greater than the height of the ith person. For a person i, all the persons from 1 to i - 1 are considered to be before him. eg, For person 2, person 1 is considered before him.</p>
<p>You have to find out whether this array can be valid for some arrangement of persons. If you can uniquely do so then output "YES" Otherwise output "NO".</p>
<h3>Input</h3>
<p>First line contains T : number of test cases. (1 &lt;= T &lt;= 20).</p>
<p>For each test First line contains an integer n. (1 &lt;= N &lt;= 10^5)</p>
<p>Next line contains n space seperated integers denoting A[i]. (0 &lt;= A[i] &lt;= N)</p>
<h3>Output</h3>
<p>For each test case, output "YES" or "NO" according to answer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>2<br>0 1<br>2<br>1 1&nbsp;</pre>
<pre><strong>Output:</strong>
YES<br>NO</pre>
<h3>Explanation</h3>
<p>&nbsp; For the first test case, [2, 1] is a valid case, First person has height 2, second person has height 1.&nbsp;</p>
<p>&nbsp; For the second test case, no valid test case exists.</p>