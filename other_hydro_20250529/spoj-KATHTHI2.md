<p><span style="font-weight: bold;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Problem Statement :</span></span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">Sathish and Kathiresan are known for Coin Fight.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">Kathiresan kept on tossing a biased coin repeatedly. Then he decided to solve the following problem.</span></span></p>
<p>&nbsp;</p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">Find the number of tosses for which the probability of getting exactly K heads is maximum. In case of a tie, return the minimum number of tosses.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">In other words, find the minimum n such that Prob (exactly K heads with n tosses) &gt;= Prob (exactly K heads with m tosses) for any m!=n.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></p>
<p><strong><span style="font-size: small;"><span style="font-family: verdana, geneva;">Input :&nbsp;</span></span></strong></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">The first line consists of an integer t, the number of test cases. For each test case you are given an integer K, the number of heads required and a float p, the probability to get a head when the coin is tossed.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></p>
<p><strong><span style="font-size: small;"><span style="font-family: verdana, geneva;">Output :</span></span></strong></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">For each test case find the number of tosses required as defined.</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></p>
<p><strong><span style="font-size: small;"><span style="font-family: verdana, geneva;">Input Constraints :</span></span></strong></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">1 &lt;= t &lt;= 100</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">1 &lt;= K &lt;= 100</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">0.00 &lt; p &lt;= 1.00</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">p will always contain 2 decimal places</span></span></p>
<p>&nbsp;</p>
<p><strong><span style="font-size: small;"><span style="font-family: verdana, geneva;">Time Limit :</span></span></strong></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">3 seconds</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></p>
<p><strong><span style="font-size: small;"><span style="font-family: verdana, geneva;">Sample Input :</span></span></strong></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">3</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">5 1.00</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">1 0.50</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">2 0.30</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></p>
<p><span style="font-size: small;"><strong><span style="font-family: verdana, geneva;">Sample Output :</span></strong></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">5</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">1</span></span></p>
<p><span style="font-size: small;"><span style="font-family: verdana, geneva;">6</span></span></p>
<p>&nbsp;</p>