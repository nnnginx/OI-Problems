<p><a href="http://www.spoj.com/users/g201513">HL</a>, <a href="http://www.spoj.com/users/lcosvse">HJ</a> and <a href="http://www.spoj.com/users/xilinx">FGD</a> set problem for <a href="http://www.spoj.com/users/zmy">ZMY</a> everyday. The title of each problem bores them very much. The title is a string which consists only lower case letters. It's length is <em>L</em>, and, of course, the title must contain their names(hl, hj, fgd) as consecutive substrings.More apparently, <em>N</em> evil consecutive substrings should not appear in the title. Any string satisfying the two conditions above is OK.</p>
<p>The task ZMY is to do today is: if they give ZMY 8 problems every week, and the title of each problem should not be repeated, how many (complete) weeks can they set problems?</p>
<h3>Input</h3>
<p>Multiple test cases.Input terminates by EOF.</p>
<p>For each test case:</p>
<p>The first line contains two space-seperated integers L(0&lt;=L&lt;=10<sup>9</sup>) and N(0&lt;=N&lt;=20). N lines follow, each contains a string (contains only lowercase letters), which is evil.You can assume the total length of the N evil strings is no more than 20.</p>
<h3>Output</h3>
<p>For each test case output one line contains the answer modudo 1000.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 1
zmy

<strong>Output:</strong>
245
</pre>