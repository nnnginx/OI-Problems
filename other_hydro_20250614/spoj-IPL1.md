<p style="text-align: center;"><span style="font-size: medium;"><strong>&nbsp;</strong></span></p>
<p>&nbsp;</p>
<p style="text-align: center;"><span style="font-size: small;"><img src="./22966/file/mkkm0ZtA.png" alt="" width="500" height="300">&nbsp;</span></p>
<p><span style="font-size: small;">NOTE: This problem needs knowledge about the game <a href="http://en.wikipedia.org/wiki/Cricket">cricket</a>.</span></p>
<p><span style="font-size: small;">Those who know the basics about IPL can skip the first paragraph.</span></p>
<p><span style="font-size: small;">IPL is one of the famous cricket tournaments. Every match is played between two teams. Each team has eleven players. When the first team bats, the second team bowls. The second team¡¯s aim is to get more score/runs than the first team and the first team¡¯s aim is to defend their score. Each team can bat either till the end of 20 overs or until they lose 10 wickets. 6 balls are bowled every over.</span></p>
<p><span style="font-size: small;">The possible things that can happen in any ball are dot-ball, 1 run, 2 runs, 3 runs, 4 runs, 5 runs,&nbsp;6 runs, wide, no-ball, wicket. For any no-ball or a wide, 1 run is granted and the ball is not counted. Assume that these things can happen with equal probability. <br> </span></p>
<p><span style="font-size: small;">You are given the overs gone, the current score/wickets and the Target. Find the winning probability of the chasing team.</span></p>
<p><span style="font-size: small;">&nbsp;</span></p>
<p><span style="font-size: small;"><strong>Input Specifications:</strong></span></p>
<p><span style="font-size: small;">The first line consists of an integer t, denoting the number of test cases. Then for the next t lines, each test case consists of three inputs. The overs, current score and the target score.</span></p>
<p><span style="font-size: small;">&nbsp;</span></p>
<p><span style="font-size: small;"><strong>Output Specifications:</strong></span></p>
<p><span style="font-size: small;">For each test case output the winning probability(in percentage) of the chasing team.</span></p>
<p><span style="font-size: small;"><strong>Note: The first two decimal places in it's representation should be printed without rounding</strong></span></p>
<p><span style="font-size: small;"><strong><br></strong></span></p>
<p><span style="font-size: x-small;"><strong><span style="font-size: small;">Input Constraints:</span></strong></span></p>
<p><span style="font-size: small;">1&lt;=t&lt;=1000</span></p>
<p><span style="font-size: small;">0.0 &lt;= Overs &lt;= 20.0</span></p>
<p><span style="font-size: small;">0&lt;= Score &lt;= 300</span></p>
<p><span style="font-size: small;">0&lt;= Wickets &lt;= 10</span></p>
<p><span style="font-size: x-small;"><span style="font-size: small;">Score &lt;= Target &lt;= 300</span><strong>&nbsp;<br></strong></span></p>
<p>&nbsp;</p>
<p><span style="font-weight: bold; font-size: small;">Sample Input:</span></p>
<p><span style="font-size: small;">10</span></p>
<p><span style="font-size: small;">19.4 129/9 129</span></p>
<p><span style="font-size: small;">20.0&nbsp;</span><span style="font-size: small;">100/10 100</span></p>
<p><span style="font-size: small;">19.5 0/9 100</span></p>
<p><span style="font-size: small;">19.5 0/0 1</span></p>
<p><span style="font-size: small;">0.0 0/0 300</span></p>
<p><span style="font-size: small;">0.0 0/0 200</span></p>
<p><span style="font-size: small;">0.0 0/0 100</span></p>
<p><span style="font-size: small;">10.0 0/0 100</span></p>
<p><span style="font-size: small;">10.0 0/5 100</span></p>
<p><span style="font-size: small;">13.5 112/4 222</span></p>
<p>&nbsp;</p>
<p><span style="font-weight: bold; font-size: small;">Sample Output:</span></p>
<p><span style="font-size: small;">100.00</span></p>
<p><span style="font-size: small;">100.00</span></p>
<p><span style="font-size: small;">0.00</span></p>
<p><span style="font-size: small;">80.00</span></p>
<p><span style="font-size: small;">18.02</span></p>
<p><span style="font-size: small;">61.65</span></p>
<p><span style="font-size: small;">97.60</span></p>
<p><span style="font-size: small;">97.60</span></p>
<p><span style="font-size: small;">55.49</span></p>
<p><span style="font-size: small;">35.84&nbsp;</span></p>