<p><span style="white-space: normal;"><span style="font-size: medium;">
</span></span></p><p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">Shoumik loves problem solving but he is weak in string related problems.&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">So he is practicing string &nbsp;related problems. But he thought that creating&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">a string related problem and solving that would be a great idea to be&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">strong in strings. So he thought of a problem.</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">Given a string S of N lower case alphabets how many distinct substrings T&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">are there with length L( L=|T| ) and S contains exactly X occurrences of T.&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">In the string S=¡°abcbcb¡± the substring T=¡°bcb¡± has length L=3 and S&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">has X=2 occurrences of T.(See hints for more clarification)</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">But as Shoumik is weak in string, he is stuck with this problem. You have&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">to help him answering Q queries for a given string S.</p>
<h3 style="text-align: left;"><span style="font-size: large;">Input</span></h3>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">First line of input will contain the number of test cases Ts.</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">Then Ts test cases follows. Every test case contains two integers</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">N and Q in the first line. Next line will contain a string S, consisting of</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">N lower casecharacters. The next Q lines will contain Q queries with</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">two integers L,length of T for this query and X, Occurrences of T in S.</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">1&lt;=Ts&lt;=15</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">1&lt;=N&lt;=10000</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">1&lt;=Q&lt;=100000</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">1&lt;=L&lt;2^31</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">0&lt;=X&lt;2^31</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">Sum of N over all test cases &lt;=60000 (6*10^4)<br>Number of queries Q over all test cases &lt;= 600000 (6*10^5)</p>
<h3 style="text-align: left;"><span style="font-size: large;">Output</span></h3>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">For every query print the number of distinct substrings  T in the string S&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: left;">which are of length L and have exactly X occurrences in S.</p>
<h3 style="text-align: left;"><span style="font-size: large;">Example</span></h3>
<pre style="text-align: left;"><span style="font-size: large;"><strong>Input:</strong></span></pre>
<pre style="text-align: left;"><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">1</span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;"><br></span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">6 5</span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;"><br></span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">abcbcb</span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;"><br></span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">3 2</span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;"><br></span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">4 1</span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;"><br></span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">6 2</span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;"><br></span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">6 1</span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;"><br></span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">1 2</span></p><span style="font-size: large;">
<strong>Output:</strong>
</span><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">1</span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;"><br></span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">3</span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;"><br></span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">0</span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;"><br></span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">1</span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;"><br></span></p><p style="margin-bottom: 0in; line-height: 100%;"><span style="font-size: large;">1</span></p><p style="margin-bottom: 0in; line-height: 100%;">&nbsp;</p></pre>
<p></p>
<h3><span style="font-size: large;">Hints</span></h3>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;"><span style="font-size: medium;"><span style="font-size: medium;">For the 2nd query we have 3 distinct substrings of length 4 ¡°abcb¡±,¡°bcbc¡±,</span></span></p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;"><span style="font-size: medium;"><span style="font-size: medium;">¡°cbcb¡± </span></span><span style="font-size: medium;">and all of them have 1 occurrence in S. So the answer is 3.</span></p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;">&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;"><span style="font-size: medium;"><span style="font-size: medium;">For the 5th query we have 3 distinct substrings of length 1 ¡°a¡±,¡°b¡±,¡°c¡± </span></span></p>
<p style="margin-bottom: 0in; line-height: 100%; text-align: justify;"><span style="font-size: medium;"><span style="font-size: medium;">but only ¡°c¡± has 2 occurrences in S. So the answer is 1.</span></span></p>