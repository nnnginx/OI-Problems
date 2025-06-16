<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">One of the largest perfume shops is making perfumes by mixing fragrant</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">essential oils with other compounds. The shop representative told you that what</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">really matters in the mixture is the percentages of two main components (call</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">them A and B), all other stuff is complementary. For example their first sold</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">perfume had 10% of component A and 35% of component B, while the most</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">successful one had 16% of A and 20% of B. Sometimes the store needs to</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">create a new mixture with specific percentages of A and B and they wonder if</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">this can be achieved by mixing some of the mixtures they already have and this</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">is where they need your help. For example a new mixture which has 12% of A</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">and 30% of B can be created by mixing the two mixtures above in the ratio 2:1,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">while it is impossible to create a mixture which has 13% of A and 22% of B</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">using the same two mixtures.</div>
<p>&nbsp;</p>
<p>One of the largest perfume shops is making perfumes by mixing fragrant&nbsp;essential oils with other compounds. The shop representative told you that what&nbsp;really matters in the mixture is the percentages of two main components (call&nbsp;them A and B), all other stuff is complementary. For example their first sold&nbsp;perfume had 10% of component A and 35% of component B, while the most&nbsp;successful one had 16% of A and 20% of B. Sometimes the store needs to&nbsp;create a new mixture with specific percentages of A and B and they wonder if&nbsp;this can be achieved by mixing some of the mixtures they already have and this&nbsp;is where they need your help. For example a new mixture which has 12% of A&nbsp;and 30% of B can be created by mixing the two mixtures above in the ratio 2:1,&nbsp;while it is impossible to create a mixture which has 13% of A and 22% of B&nbsp;using the same two mixtures.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line contains T &lt;= 100, the number of test cases. The first line of each&nbsp;test case contains an integer (1 &lt;= N &lt;= 200), the number of mixtures the shop&nbsp;already has. The next N lines each contain two floating point numbers (0 &lt;= A,&nbsp;B &lt;= 100, A+B &lt;= 100) representing the percentages of components A and B in&nbsp;each mixture. The next line contains an integer (1 &lt;= Q &lt;= 5151) the number&nbsp;of mixtures to verify. The next Q lines each contain two floating point numbers&nbsp;(0 &lt;= A, B &lt;= 100, A+B &lt;= 100) representing the percentages of components&nbsp;A and B in each new mixture. Test cases are separated by one or more empty&nbsp;lines.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each mixture query print "Yes" if the new mixture can be created from the&nbsp;already existent ones or "No" otherwise. Print a blank line between test cases.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
2
10.0000 35.0000
16.0000 20.0000
2
12.0000 30.0000<br>13.0000 22.0000<br>
3
10 35
16 20
7 15
1
13 22

<strong>Output:</strong>
Yes
No<br><br>Yes</pre>