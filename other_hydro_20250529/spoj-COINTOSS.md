<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">You have an unbiased coin which you want to keep tossing till you get N consecutive heads. You've already tossed the coin M times already and surprisingly, all tosses resulted in heads. What is the expected number of tosses needed till you get N consecutive heads?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For example, if N = 2 and M = 0. You need to keep tossing the coin till you get 2 consecutive heads. It is not hard to show that on an average, 6 coin tosses are needed.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">As another example, if N = 2 and M = 1. You need 2 consecutive heads and have already got 1. In your first toss, if you get get a heads, you are done. Otherwise, you need to keep tossing the coin till you get 2 consecutive heads. The expected number of coin tosses is thus 1 + (0.5 * 0 + 0.5 * 6) = 4.0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains the number of cases T. Each of the next T lines contains two numbers N and M.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output T lines containing the answer for the corresponding test case. Print the answer rounded to exactly 2 decimal places.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= T &lt;= 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= N &lt;= 1000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 &lt;= M &lt;= N</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">6.00</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4.00</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0.00</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">8.00</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Explanation:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first two samples are explained above. For the third case, you already have got 3 heads, so you do not need any more tosses.</div>
<p>&nbsp;</p>
<p>You have an unbiased coin which you want to keep tossing till you get N consecutive heads. You've already tossed the coin M times already and surprisingly, all tosses resulted in heads. What is the expected number of tosses needed till you get N consecutive heads?</p>
<p>&nbsp;</p>
<p>For example, if N = 2 and M = 0. You need to keep tossing the coin till you get 2 consecutive heads. It is not hard to show that on an average, 6 coin tosses are needed.</p>
<p>&nbsp;</p>
<p>As another example, if N = 2 and M = 1. You need 2 consecutive heads and have already got 1. In your first toss, if you get get a heads, you are done. Otherwise, you need to keep tossing the coin till you get 2 consecutive heads. The expected number of coin tosses is thus 1 + (0.5 * 0 + 0.5 * 6) = 4.0</p>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p>The first line contains the number of cases T. Each of the next T lines contains two numbers N and M.</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>Output T lines containing the answer for the corresponding test case. Print the answer rounded to exactly 2 decimal places.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 100</p>
<p>1 &lt;= N &lt;= 1000</p>
<p>0 &lt;= M &lt;= N</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>4</p>
<p>2 0</p>
<p>2 1</p>
<p>3 3</p>
<p>3 2</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>6.00</p>
<p>4.00</p>
<p>0.00</p>
<p>8.00</p>
<p>&nbsp;</p>
<p><strong>Explanation:</strong></p>
<p>The first two samples are explained above. For the third case, you already have got 3 heads, so you do not need any more tosses.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>