<p>Maggu and Coder were playing a game with strings. In each turn of the game, Maggu gives Coder a string. Coder can replace m consecutive 'a' in the string by n consecutive 'b' any number of times. This way he has to create 2 strings, one of maximum possible length and one of minimum possible length.</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Maggu and Coder were playing a game with strings. In each turn of the game, Maggu gives Coder a string. Coder can replace m consecutive 'a' in the string by&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">n consecutive 'b' any number of times. This way he has to create 2 strings, one of maximum possible length and one of mimimum possible length.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp;&nbsp;</div>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line of input contains a single integer T : number of test cases.(1&lt;=T&lt;=100).<br>For each test case there are exactly two lines.<br>First line contains a string s (1 &lt;= length(s) &lt;= 10^5) containing letters only from 'a' to 'z'.<br>Second line contains two space separated integers representing m and n respectively.(1 &lt;= m,n &lt;= 10^5).<br>Sum of length(s) over all test cases is &lt;= 10^6.&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print in a single line containing two space separated integers representing minimum and maximum length of string s that Coder can obtain.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>abc<br>1 2<br>aa<br>1 2<br>aba<br>1 1

<strong>Output:</strong>
3 4<br>2 4<br>3 3</pre>
<h3>Explanation</h3>
<p>For the first test case, you can convert abc to abc (by not changing at all), bbbc (changing 'a' to 'bb'). minimum length of s is 3 and maxium length is 4.</p>