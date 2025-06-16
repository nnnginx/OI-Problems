<p>&nbsp;</p>
<p><span style="font-size: small;"><span style="line-height: 21px;">&nbsp;</span></span></p>
<p style="text-align: left;"><span style="font-size: small;">On a sunny day, Stjepan and Bobert were arguing over their problem solving skill under a big apple tree. Bobert brought up a nice problem he had just recently solved and claimed that Stjepan could not solve it. Stjepan is desperate and needs your help. Here is Bobert's problem:</span></p>
<p style="text-align: left;"><span style="font-size: small;">Given an array of <strong>N</strong> (1 &lt;= N &lt;= 10^5) numbers (0 &lt;= <strong>ai</strong> &lt;= 10^9) and <strong>K</strong> (1 &lt;= K &lt;= 20) sticks of a certain length <strong>Li</strong> (0 &lt;= Li &lt;= N, &nbsp;such that the sum of all lengths is equal to N), find the best possible distribution of the sticks among the array such that:</span></p>
<div style="text-align: left;"><span style="font-size: small;">&nbsp;</span></div>
<div style="text-align: left;"><span style="font-size: small;">1) a stick of length L<sub>x</sub> can cover any interval of the array whose length is equal to the length of the stick (it can cover L<sub>x</sub> consecutive numbers of the array)</span></div>
<div style="text-align: left;"><span style="font-size: small;">&nbsp;</span></div>
<div style="text-align: left;"><span style="font-size: small;">2) all sticks must be used and can not overlap or leave the borders of the array&nbsp;</span></div>
<div style="text-align: left;"><span style="font-size: small;">&nbsp;</span></div>
<div style="text-align: left;"><span style="font-size: small;">3) the value of a stick of length L<sub>x</sub> covering the interval [lo, hi] is equal to: L<sub>x</sub> * (max[lo, hi] - min[lo, hi])</span></div>
<div style="text-align: left;"><span style="font-size: small;">Note that:&nbsp;</span><span style="font-size: small;">max = largest element of the array inside the interval and&nbsp;</span><span style="font-size: small;">min = smallest element of the array inside the interval</span></div>
<div style="text-align: left;"><span style="font-size: small;">&nbsp;</span></div>
<div style="text-align: left;"><span style="font-size: small;">4) the sum of all stick values must be as large as possible</span></div>
<p>&nbsp;</p>
<p><strong>Note: </strong>double-check your complexity</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 317px; width: 1px; height: 1px; overflow: hidden;">9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 317px; width: 1px; height: 1px; overflow: hidden;">2 6 3 1 8 4 3 5 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 317px; width: 1px; height: 1px; overflow: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 317px; width: 1px; height: 1px; overflow: hidden;">2 3 2 2</div>
<p>The first line contains an integer N.&nbsp;</p>
<p>The second line contains N numbers representing the array.</p>
<p>The third line contains an integer K.</p>
<p>The fourth line contains K numbers representing the stick lengths.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>The only line should contain the solution - the maximum sum of stick values as explained in the task.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
9
2 6 3 1 8 4 3 5 6
4
2 3 2 2

<strong>Output:</strong>
33</pre>