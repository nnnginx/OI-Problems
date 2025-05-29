<p>A string is called a "prime string" if it can't be written as  concatenation of more than one same strings. For example, the following  strings are not prime strings: AAA, ABABAB, CFGFGCFGFG, while CFGFGC,  ABABA are prime strings. <br> Calculate the number of prime string of length N  (1&lt;=N&lt;=1000000), and only contains first K (1&lt;=K&lt;=26)  letters from English alphabet. Note that some of these K letters need  not appear in that string.</p>
<h3>Input</h3>
<p>Multiple test cases. The number of them (about 10000) is given in the very first line. <br> Each test case contains one line with two integers - K and N, seperated by a single space.</p>
<h3>Output</h3>
<p>For each test case, output the required number modulo 1000000007 in a single line.</p>
<p>Example</p>
<pre><strong>Input:</strong><br>1<br>2 3<br><strong>Output:</strong><br>6<br><strong>Explanation<br></strong>The prime strings of length 3 which only contain character 'A' and 'B' are: AAB,ABA,ABB,BAA,BAB,BBA.<br></pre>
<h3>Constraints</h3>
<p>1 &lt;= N &lt;= 1000000                     1 &lt;= K &lt;= 26<br> Total number of test cases is around 10000.</p>