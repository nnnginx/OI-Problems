<p>Little Willy just took a compilers course and is trying to implement his own compiler. First he wants to build a table with all the possible ids that a program could have. He knows that his language supports up to N different characters and any id can be up to L characters long. For example, when N = 2 (lets say characters can be 0 or 1), and L = 3, he could have the following ids: {0, 1, 00, 01, 10, 11, 000, 001, 010, 011, 100, 101, 110, 111}.</p>
<p>You have to write a program that can help Willy find out the size of the table. Since the answer can be really big, you must print it modulo 1000000007 (10^9+7).</p>
<h3>Input</h3>
<p>The input contains several test cases. Each test case will consist of a single line containing two integers N and L. N is the number of characters that can be part of an id and L is maximum lenght supported by the language (1 &lt;= N &lt;= 65535, 1 &lt;= L &lt;= 10^5).</p>
<p>End of the input is indicated by a test case with N = 0, L = 0 that should not be processed.</p>
<h3>Output</h3>
<p>For each test case output a single line containing the number of possible ids modulo 10^9+7.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 3<br>128 32<br>0 0

<strong>Output:</strong>
14<br>792805767</pre>