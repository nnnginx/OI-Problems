<p>Given a string, we need to find the total number of its distinct substrings.</p>
<h3>Input</h3>
<p>T- number of test cases. T&lt;=20;<br>
Each test case consists of one string, whose length is &lt;= 1000</p>
<h3>Output</h3>
<p>For each test case output one number saying the number of distinct substrings.</p>

<h3>Example</h3>
<tt>
<p><strong>Sample Input:</strong><br>
  2<br>
  CCCCC<br>
  ABABA</p>
<p><strong>Sample Output:</strong><br>
  5<br>
  9</p>
</tt>

<p>Explanation for the testcase with string ABABA: <br>
  len=1 : A,B<br>
  len=2 : AB,BA<br>
  len=3 : ABA,BAB<br>
  len=4 : ABAB,BABA<br>
  len=5 : ABABA<br>

  Thus, total number of distinct substrings is 9.<br>
</p>