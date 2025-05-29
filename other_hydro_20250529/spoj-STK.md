<p>Alex heard a lot about investing in the stock market and now wants to do it to earn some profit. Being a new investor he is scared of the risks in the stock market, so he decides that at any instance he will not have more than one stock with him. It is also decided that on a particular day he can either buy or sell atmost one stock(only one transaction allowed). Now given the prices of one particular stock over the period of n days Alex decides he will make atmost k buys and k sells.</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Alex heard a lot about investing in the stock market and now wants to do it to earn some profit. Being a new</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">investor he is scared of the risks in the stock market, so he decides that at any instance he will not have more</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">than one stock with him. It is also decided that on a particular day he can either buy or sell atmost one stock(only one transaction allowed).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Now given the prices of one particular stock over the period of n days Alex decides he will make atmost k buys and</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">k sells.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Write a code to help Alex to maximize his profit.</div>
<p>Write a code to help Alex to maximize his profit.</p>
<h3>Input</h3>
<p>First line contains an integer T(&lt;=100), number of test cases.</p>
<p>Each test case will have n(&lt;=3000) and k(1&lt;=k&lt;=n/2), is the no. of days and the maximum buys/sells allowed respectively.</p>
<p>(Value of the prices are in range of unsigned 32-bit integer.)</p>
<p>Next line will have n space separated integers denoting the price of stock over n days.</p>
<h3>Output</h3>
<p>For each test case output one line stating the maximum profit.</p>
<h3>Example</h3>
<pre>Sample Input:

3
10 3
2 7 3 9 8 7 9 7 1 9
10 1
2 7 3 9 8 7 9 7 1 3
10 2
2 7 3 9 8 7 9 7 1 9
	
Sample Output:
	
19 
7
15

Explanation:
1st test case Alex would buy on 1st day and sell it on the 2nd day, and then buy another on the 3rd day and sell it on the
4th, finally buys on 9th day and sells on the 10th day.So profit = (7-2)+(9-3)+(9-1) = 19.

2nd test case Alex would buy on 1st day and sell it on the 4th(or 7th) day. So profit = 9-2 = 7.

2nd test case Alex would buy on 1st day and sell it on the 4th day, and then buy another on the 9th day and sell it on the
10th day.So profit = (9-2)+(9-1) = 15.</pre>