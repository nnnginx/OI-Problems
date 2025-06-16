<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">abdou has a set of unique positive integers . he wants to add several (possibly none) new positive integers to this set, such that when the set is sorted for every two consecutive numbers X , Y we have abs(X%m-Y%m) = 1 . your task is to calculate the smallest possible count of new numbers, with which he can achieve that.&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Input</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">The first line contains T, the number of test cases. It is followed by 2*T each test case consist of two lines the first line contain two numbers m , N .. the second line contain N integer .</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1 &lt;=T &lt;= 5000 .</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1 &lt;= m &lt;= 10^5&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">2 &lt;= N &lt;=50.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1 &lt;= every integer in the set &lt;= 10^6</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Output</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">&nbsp;For each line of input produce one line of output. This line contains the smallest possible count of new numbers, with which he can complete the set &nbsp;or -1 if no solution .</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Example</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">input</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">5</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">2 3&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">2 10 20</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">10 2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">10 20</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">10 6</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">11 19 5 30 40 100</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1 2&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1 &nbsp;9999</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">15 3</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">4218 15210 1426</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">10 6 11 19 5 30 40 1007</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">output</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">2</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">-1</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">-1</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">3</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">expanation :</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">in first test case we can add 3 and 13 to the given set to &nbsp;achieve abdou goal &nbsp;.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">you can see my time here&nbsp;</span></div>
<p>&nbsp;</p>
<p><span style="font-size: small;"><a href="../../../users/abdou_93/">Abdou</a> has a set of unique positive integers. He wants to add several (possibly none) new positive integers to this set, such that when the set is sorted, for every two consecutive numbers X , Y abs(X%M-Y%M) = 1 . Your task is to calculate the smallest possible count of new numbers, with which he can achieve that.&nbsp;</span></p>
<p><span style="font-size: small;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;<strong>Input</strong></span></p>
<p><span style="font-size: small;">The first line contains T, the number of test cases. It is followed by 2*T lines, two lines per test case. The first line contains two positive integers M and N. The second line contains N integers.</span></p>
<p><span style="font-size: small;">1 &lt;= T &lt;= 5000 .</span></p>
<p><span style="font-size: small;">1 &lt;= M &lt;= 10^5&nbsp;</span></p>
<p><span style="font-size: small;">2 &lt;= N &lt;=50.</span></p>
<p><span style="font-size: small;">1 &lt;= every integer in the set &lt;= 10^6</span></p>
<p><span style="font-size: small;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <strong>Output</strong></span></p>
<p><span style="font-size: small;">For test case print a single integer in a separate line: the smallest possible count of new numbers, with which he can complete the set or -1 if no solution exists.</span></p>
<p><span style="font-size: small;">&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; <strong>Example</strong></span></p>
<p>
</p><p><span style="font-size: small;"><strong>Input:</strong></span></p>
<p><span style="font-size: small;">5</span></p>
<p><span style="font-size: small;"><span style="font-size: small;">2 3&nbsp;</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">2 10 20</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">10 2</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">10 20</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">10 6</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">11 19 5 30 40 100</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">1 2&nbsp;</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">1 &nbsp;9999</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">15 3</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">4218 15210 1426</span></span></p>
<br>
<p><span style="font-size: small;"><strong>Output:</strong></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">2</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">1</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">-1</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">-1</span></span></p>
<p><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">3</span></span></p>
<br>
<p><span style="font-size: small;"><b>Explanation:</b></span></p>
<p><span style="font-size: small;">In the first test case we can add 3 and 13 to the given set to achieve abdou goal.</span></p>
<br>