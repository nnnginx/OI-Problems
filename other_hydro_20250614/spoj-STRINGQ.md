<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Consider a string S, consisting of lowercase alphabets.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You are given a list of queries, each of which belong to one of the following two types:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1) Q a b: Returns the number of ways of rearranging the alphabets in the substring [a,b] such that for each substring X in the resulting string A, Reverse(X) is also present in A. Reverse(X) prints the string X in reverse.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2) U a b: Sorts the substring [a,b] lexicographically.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Thus, given the string S and a list of queries, print the answer for each query of type 1. Since the answer can be huge, print the result modulo 106109099.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Finally, output the string S, with the updations made, if any.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Note: Two ways of rearranging the alphabets are considered different if, for two resulting strings A, B you can find an index i such that A[i] != B[i].</div>
<p>&nbsp;</p>
<p>Consider a string S, consisting of lowercase alphabets.</p>
<p>You are given a list of queries, each of which belong to one of the following two types:</p>
<p>1) Q a b: Returns the number of ways of rearranging the alphabets in the substring [a,b] such that for each substring X in the resulting string A, Reverse(X) is also present in A. Reverse(X) reverses the string X.</p>
<p>2) U a b: Sorts the substring [a,b] lexicographically.</p>
<p>&nbsp;</p>
<p>Thus, given the string S and a list of queries, print the answer for each query of type 1. Since the answer can be huge, print the result modulo 106109099.</p>
<p>Finally, output the string S, with the updations made, if any.</p>
<p>Note: Two ways of rearranging the alphabets are considered different if, for two resulting strings A, B you can find an index i such that A[i] != B[i].</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>&nbsp; &nbsp;First line contains T, the number of test cases.</p>
<p>&nbsp; &nbsp;For each test case, first line contains S, the input string.</p>
<p>&nbsp; &nbsp;Next line contains N, the number of queries. Each of the next N lines contains a string of the form "X a b" where X is one of {"Q","U"} and a and b are positive integers such that &nbsp; &nbsp;1&lt;=a&lt;=b&lt;=|S|.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>&nbsp; &nbsp;For each test case, print X+1 lines, where X is the number of queries of type Q.</p>
<p>&nbsp; &nbsp;For each query of type Q, print one number which is the answer to the query.</p>
<p>&nbsp; &nbsp;(X+1)th line for each test case, should contain the updated string S.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3><span style="font-size: 12px;">Constraints:</span></h3>
<h3 style="text-align: left;"><span style="font-weight: normal;"><span style="font-size: x-small;">&nbsp; &nbsp;1 &lt;= T &lt;= 10</span></span></h3>
<h3 style="text-align: left;"><span style="font-weight: normal;"><span style="font-size: x-small;">&nbsp; &nbsp;1 &lt;= |S| &lt;= 50000</span></span></h3>
<h3 style="text-align: left;"><span style="font-weight: normal;"><span style="font-size: x-small;">&nbsp; &nbsp;1 &lt;= N &lt;= 2000</span></span></h3>
<p style="text-align: left;">&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>2
nittirichy
3
Q 2 5
U 1 4
Q 1 5
shabba
5
Q 2 3
Q 2 6
U 1 4
Q 2 5
Q 1 6

<strong>Output:</strong>
</pre>
<pre>2
2
inttirichy
0
2
0
0
abhsba</pre>