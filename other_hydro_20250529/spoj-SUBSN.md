<p style="text-align: justify;">&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden; text-align: justify;">A subsequence is a sequence that can be derived from another sequence by deleting some</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden; text-align: justify;">elements without changing the order of the remaining elements. For example ¡°abd¡± is a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden; text-align: justify;">subsequence of ¡°abcdef¡±. - Wikipedia</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden; text-align: justify;">Your task in this problem is to decide if a given string is a subsequence of another string or not?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden; text-align: justify;">Easy?</div>
<p style="text-align: justify;">A subsequence is a sequence that can be derived from another sequence by deleting some elements without changing the order of the remaining elements. For example ¡°abd¡± is a subsequence of ¡°abcdef¡±. - Wikipedia.</p>
<p style="text-align: justify;">Your task in this problem is to decide if a given string is a subsequence of another string or not?</p>
<p style="text-align: justify;">Easy?</p>
<h3 style="text-align: justify;">Input</h3>
<p style="text-align: justify;">The first line of input will be the number of test cases. Each test case will start with a line contains a string S, S will have letters from 'a' to 'z' and the length of S &lt;= 100,000. This line will be followed by a number Q which is the number of queries you have to answer for the given string S, 1 &lt;= Q &lt;= 1000. Each of the next Q lines will contain a string T, T will have letter from 'a' to 'z' and the length of T &lt;= 200. For each T you have to decide if T is a subsequence of S or not.</p>
<h3 style="text-align: justify;">Output</h3>
<p style="text-align: justify;">For each test case print Q + 1 lines, The first line will have ¡°Case C:¡± without quotes where C is the case number starting with 1. The next Q lines will have either ¡°YES¡± or ¡°NO¡± if the cross-ponding T is a subsequence of S or not respectively.</p>
<h3>Example</h3>
<pre><strong><u>Input:</u></strong>
1
abcdef
3
abd
adb
af

<strong><u>Output:</u></strong>
Case 1:
YES
NO
YES</pre>

<br>
<p><b><u>Editors note:</u></b><br>
Strings in the input can be empty. Read data carefully to avoid issues. There should be no extra withespaces, of course except '\n'.</p>