<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">You are given a sequence of numbers s, you are required to find 3 indices i, j, k, where i &lt; j &lt; k and (s[i] &lt;= s[j] &gt;= s[k] or s[i] &gt;= s[j] &lt;= s[k]) if there are many solutions you should find the one where |s[i]-s[j]| + |s[j]-s[k]| is maximized, if there are still many solutions you should find the one which comes earlier in order (i.e. i1, j1, k1, comes before i2, j2, k2, if i1&lt;i2, or if i1=i2, and j1&lt;j2, or if i1=i2, j1=j2, and k1&lt;k2 ).</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Input Specification</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">The problem will be tested on multiple test cases, the first line of the input contains an integer n representing the size of the sequence (3&lt;=n&lt;=10^6) (^ means power), then followed by n integers, All numbers in this sequence do not exceed 10^6 in absolute value. The input is terminated by end of file.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Output Specification</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">For each test case, output a line containing the 3 indices of the pattern i, j, k space separated. If there is no such pattern output -1 instead.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Sample Input</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">7</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">2 3 1 7 2 4 8</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">5</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">2 3 5 7 1</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">Sample Output</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">3 4 5</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">1 4 5</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"><span style="font-size: small;">&nbsp;</span></div>
<p>&nbsp;</p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;">You are given a sequence of numbers s, you are required to find 3 indices i, j, k, where i &lt; j &lt; k and (s[i] &lt;= s[j] &gt;= s[k] or s[i] &gt;= s[j] &lt;= s[k]) if there are many solutions you should find the one where |s[i]-s[j]| + |s[j]-s[k]| is maximized, if there are still many solutions you should find the one which comes earlier in order (i.e. i1, j1, k1, comes before i2, j2, k2, if i1&lt;i2, or if i1=i2, and j1&lt;j2, or if i1=i2, j1=j2, and k1&lt;k2 ).</span></p>
<p><strong><span style="font-size: small;">Input Specification</span></strong></p>
<p><span style="font-size: small;">The problem will be tested on multiple test cases, the first line of the input contains an integer n representing the size of the sequence (3&lt;=n&lt;=10^6) (^ means power), then followed by n integers, All numbers in this sequence do not exceed 10^6 in absolute value. The input is terminated by end of file.</span></p>
<p><strong><span style="font-size: small;">Output Specification</span></strong></p>
<p><span style="font-size: small;">For each test case, output a line containing the 3 indices of the pattern i, j, k space separated. If there is no such pattern output -1 instead.</span></p>
<p><strong><span style="font-size: small;">Sample Input</span></strong></p>
<p><span style="font-size: small;">7</span></p>
<p><span style="font-size: small;">2 3 1 7 2 4 8</span></p>
<p><span style="font-size: small;">5</span></p>
<p><span style="font-size: small;">2 3 5 7 1</span></p>
<p><strong><span style="font-size: small;">Sample Output</span></strong></p>
<p><span style="font-size: small;">3 4 5</span></p>
<p><span style="font-size: small;">1 4 5</span></p>
<p><span style="font-size: small;">&nbsp;</span></p>
<p>&nbsp;</p>
<p>&nbsp;</p>