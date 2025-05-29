<p style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">Bubbleworld is in trouble and our wonderwoman, Billi needs to rescue the prince so as to save the kingdom from the wrath of the monster Kaddu. To do this, she needs to choose&nbsp;<span style="font-weight: 600;">K</span>&nbsp;words from a pot of&nbsp;<span style="font-weight: 600;">M</span>&nbsp;words she stole from Kaddu, and convert them to magical words, which she would use as a spell to break into the prison. She already knows&nbsp;<span style="font-weight: 600;">N</span>&nbsp;magical words.</p>
<p style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">The conversion of a stolen word to magical word requires the following operations :</p>
<p style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">1) Remove a character from the end of the word, which incurs a cost of&nbsp;<span style="font-weight: 600;">A</span>&nbsp;coins<br>2) Add a character to the end, which incurs a cost of&nbsp;<span style="font-weight: 600;">B</span>&nbsp;coins.</p>
<p style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">Help Billi save the kingdom by minimizing the cost required to convert&nbsp;<span style="font-weight: 600;">exactly K</span>&nbsp;stolen words to magical words.</p>
<h3>Input</h3>
<p style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">First line of every test file contains the number of test cases, T.<br>For each test case, first line contains 5 integers : A, B, K, N, M<br>The next N lines contain a string each, denoting the set of magical words known to Billi.<br>The next M lines contain a string each, denoting the set of words stolen from Kaddu.</p>
<h3>Constraints</h3>
<p><span style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">T &lt;= 20</span><br style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"=""><span style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">1 &lt;= N &lt;= 10000</span><br style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"=""><span style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">1 &lt;= M &lt;= 10000</span><br style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"=""><span style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">1 &lt;= K &lt;= M</span><br style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"=""><span style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">1 &lt;= A,B &lt;= 1000</span><br style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"=""><span style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">Length of each string &lt;= 100</span><br style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"=""><span style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">The strings consist of only&nbsp;</span><span style="font-weight: 600; color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">lowercase</span><span style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">&nbsp;characters.</span></p>
<h3>Output</h3>
<p><span style="color: #252c33; font-family: " open="" sans",="" sans-serif;="" font-size:="" 14px;="" word-spacing:="" 1px;"="">For each test case, print the minimum cost for the task in a single line.</span></p>
<h3>Example</h3>
<h4>Input</h4>
<pre>2
2 3 1 1 1
abc
bca
2 3 2 5 4
harry
potter
abcde
qqwweerr
ab
abc
abcd
qqwwweer
putter</pre>

<h4>Output</h4>
<pre>15
5</pre>