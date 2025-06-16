<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">One of the basics of Computer Science is knowing how numbers are represented in 2's complement. Imagine that you write down all numbers between A and B in 2's complement representation using 32 bits. How many 1's will you write down in all ?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains the number of test cases T. Each of the next T lines contains two integers A and B.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output T lines, one corresponding to each test case.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">-2^31 &lt;= A &lt;= B &lt;= 2^31 - 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">-2 0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">-3 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">-1 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">63</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">99</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">37</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For the first case, -2 contains 31 1's followed by a 0 whereas -1 contains 32 1's. Thus the total is 63.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For the second case, the answer is 31 + 31 + 32 + 0 + 1 + 1 + 2 + 1 = 99</div>
<p>One of the basics of Computer Science is knowing how numbers are represented in 2's complement. Imagine that you write down all numbers between A and B in 2's complement representation using 32 bits. How many 1's will you write down in all ?</p>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p>The first line contains the number of test cases T. Each of the next T lines contains two integers A and B.</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>Output T lines, one corresponding to each test case.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>-2^31 &lt;= A &lt;= B &lt;= 2^31 - 1</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>3</p>
<p>-2 0</p>
<p>-3 4</p>
<p>-1 4</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>63</p>
<p>99</p>
<p>37</p>
<p>&nbsp;</p>
<p><strong>Explanation</strong>:</p>
<p>For the first case, -2 contains 31 1's followed by a 0 whereas -1 contains 32 1's. Thus the total is 63.</p>
<p>For the second case, the answer is 31 + 31 + 32 + 0 + 1 + 1 + 2 + 1 = 99</p>
<p>&nbsp;</p>