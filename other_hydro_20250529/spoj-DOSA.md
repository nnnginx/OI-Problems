<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Lalith is going to have dinner and he has &nbsp;N dosas in front of him with their prices represented by sequence of integers a1,a2,a3...an.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">And he has decided to eat in a different manner . You are free to replace the price of any dosa with any positive integer.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">How many prices(integers) must be replaced to make the resulting sequence strictly increasing?</div>
<p>Lalith is going to have dinner and he has &nbsp;N dosas in front of him with their prices represented by sequence of integers a1,a2,a3...an.&nbsp;</p>
<p>And he has decided to eat in a different manner . You are free to replace the price of any dosa with any positive integer.&nbsp;</p>
<p>How many prices(integers) must be replaced to make the resulting sequence strictly increasing?</p>
<div></div>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line of the test case contains an integer N - the number of dosas.</p>
<p>The next line contains N space separated integers where the ith integer is ai , representing thr price of i-th dosa.</p>
<div></div>
<h3>Output</h3>
<p>Output the minimal number of prices(integers) that should be replaced to make the sequence strictly increasing.</p>
<div></div>
<p><strong>Constraints</strong></p>
<p>0 &lt; N &lt;= 10^6</p>
<p>0 &lt; ai &lt;= 10^9</p>
<p>&nbsp;</p>
<p><strong>Sample Input</strong> #01</p>
<p>6</p>
<p>1 7 10 2 20 22</p>
<p><strong>Sample Output</strong> #01</p>
<p>1</p>
<p>&nbsp;</p>
<p><strong>Sample Input</strong> #02</p>
<p>5</p>
<p>1 2 2 3 4&nbsp;</p>
<p><strong>Sample Output</strong> #02</p>
<p>3</p>
<p><strong>Explanation</strong>&nbsp;</p>
<p>In the first sample input, we can replace 2 with any integer between 11 and 19 to make the price sequence strictly increasing, hence the output is 1.&nbsp;</p>
<p>In the second sample input, we can obtain 1, 2, 3, 4, 5 by changing the last three elements of the price sequence.</p>
<p>&nbsp;</p>