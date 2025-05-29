<p>In this problem, a string only consists of lowercase letters.</p>
<p>Substring, is a consecutive sequence of characters occurrences at least once in a string.</p>
<p>Common substring means a substring of two strings.</p>
<p>After getting TLE on LCS and LCS2, lqp18_31 felt really depressed. So he came up with an interesting idea. He want to modify the definition of LCS and call it ELCS.</p>
<p>ELCS: for two given strings s1[0��n-1] and s2[0��m-1], the ELCS of them is a string p[0��k-1]&nbsp; k&lt;=min(n,m) so that s1[i]=s2[i]=p[i] ( for 0&lt;=i&lt;k ) and s1[k]!=s2[k] or k==n or k==m .</p>
<p>Now your task is easy.</p>
<p>You are given N strings and Q queries.</p>
<p>Each query consists two intergers a and b. You must answer the length of the ELCS of the a-th string and b-th string.</p>
<h3>Input</h3>
<p>Firtst line consists one interger N.</p>
<p>Next N lines consist N strings.</p>
<p>Next one line consists one interger Q.</p>
<p>Next Q lines consist two intergers a and b. (0&lt;=a,b&lt;N)</p>
<p>30% of the testdata : N&lt;=100 Q&lt;=10000 length(string[i])&lt;=100</p>
<p>100% of the testdata : the number of total characters&lt;=500000 N&lt;=100000 Q&lt;=100000</p>
<h3>Output</h3>
<p>Q lines. Each line consists the length of the ELCS of the a-th string and b-th string</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br><strong><p>5</p><p>dy</p><p>ljq</p><p>lqp</p><p>ws</p><p>jzt</p><p>3</p><p>0 1</p><p>1 2</p><p>0 2</p>Output:</strong><br><p>0</p><p>1</p><p>0</p></pre>