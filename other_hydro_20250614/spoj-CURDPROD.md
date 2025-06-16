<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">A curd manufacturing factory owns curd producing machines of different qualities. A curd producer of quality q produces 1 unit of curd in q units of time.</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br>For example, a curd producer of quality 5 produces 1 unit of curd at time 5, 1 unit of curd at time 10 and so on..</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Given the qualities of all the machines, find the minimum time required to produce T units of curd.</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><strong><span style="font-family: verdana, geneva;">Input:</span></strong></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">The first line consists of an integer t, the number of test cases. For each testcase, the first line consists of 2 integers n and T, the number of machines and the target amount of curd. The next n lines consists of integers representing the qualities of the producer machines.<br><strong>&nbsp;</strong></span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><strong><span style="font-size: small;"><span style="font-family: verdana, geneva;">Output:</span></span></strong></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">For each test case, find the minimum time required to produce the target amount of curd.</span></span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><strong><span style="font-size: small;"><span style="font-family: verdana, geneva;"><strong>Input Constraints</strong>:</span></span></strong></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">1 &lt;= t &lt;= 10^2</span></span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">1 &lt;= n &lt;= 10^4</span></span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">1 &lt;= T &lt;= 10^9</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">1 &lt;= quality of each machine &lt;= 10^9</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><strong>Note:</strong>&nbsp;Note that a quality 5 producer produces only 1 curd at time 9 and not 1.8.</span></span></p>
<div><strong><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></strong></div>
<p style="text-align: left;"><span style="font-size: small;"><strong><strong><span style="font-size: small;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Sample Input:</span></span></span></strong></strong></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">3</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">2 3</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">5</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">10</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">3 1000000</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">1</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">2</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">3</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">1 1000000000</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">1000000000</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-weight: bold;"><strong><span style="font-size: small;"><span style="font-family: verdana, geneva;">Sample Output:</span></span></strong></span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">10</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">545455</span></span></p>
<p style="text-align: left;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">1000000000000000000</span></span></p>