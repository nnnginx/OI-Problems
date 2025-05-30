<h2>Phone List</h2>
<p>
Given a list of phone numbers, determine if it is consistent in the
sense that no number is the prefix of another. Let��s say the phone
catalogue listed these numbers:</p>

<ul>
  <li>Emergency 911</li>
  <li>Alice 97 625 999</li>
  <li>Bob 91 12 54 26</li>
</ul>

<p>In this case, it��s not possible to call Bob, because the central would
direct your call to the emergency line as soon as you had dialled the
first three digits of Bob��s phone number. So this list would not be
consistent.</p>

<h3>Input</h3>
<p>The first line of input gives a single integer, 1 &lt;= <var>t</var> &lt;= 40, the number of test cases. Each test case starts with <var>n</var>, the number of phone numbers, on a separate line, 1 &lt;= <var>n</var> &lt;= 10000.
Then follows <var>n</var> lines with one unique phone number on each line. A phone number is a sequence of at most ten digits.

</p><h3>Output</h3>
<p>For each test case, output ��<tt>YES</tt>�� if the list is consistent, or ��<tt>NO</tt>�� otherwise.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
3
911
97625999
91125426
5
113
12340
123440
12345
98346

<b>Output:</b>
NO
YES</pre>