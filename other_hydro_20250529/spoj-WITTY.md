<p><strong>Problem Statement:</strong></p>
<p>N witty friends went for an outing trip. During the outing they have spent lot of money in lot of places. In some places, a friend (A) spends ¡®M¡¯ money for his friend (B).</p>
<p>An expense is described by&nbsp; "A spends M$ for B"</p>
<p>A transaction is described by ¡°X gives K$ to Y¡±</p>
<p>You are given all the expenses made by the friends. The outing trip is ended and now you have to find the minimum transactions to be made by the friends to tally the expenses.</p>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p>The first line consists of an integer t, the number of testcases. For each test case, the first line consists of an integer N, the number of expenses made by friends followed by N lines. Each line contains two strings A and B (A!=B) and an integer m, the money A spent for B.</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>For each test case, print the minimum number of transactions required to tally the expenses.</p>
<p>&nbsp;</p>
<p><strong>Input Constraints:<br></strong></p>
<p>1&lt;=t&lt;=10000</p>
<p>1&lt;=N&lt;=10</p>
<p>A!=B</p>
<p>Each character in A is either 'A' or 'B'</p>
<p>Each character in B is either 'A' or 'B'</p>
<p>1&lt;= length of A,B &lt;=2</p>
<p>1&lt;=m&lt;=10000</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>&nbsp;</p>
<p>3</p>
<p>1</p>
<p>AA BB 10</p>
<p>3</p>
<p>A BB 100</p>
<p>BB AA 100</p>
<p>AA A 100</p>
<p>4</p>
<p>AB BA 100</p>
<p>BA B 100</p>
<p>AB B 100</p>
<p>B A 200</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>1</p>
<p>0</p>
<p>1<br><br><strong>Explanation of Testcases</strong>:</p>
<p>Case 1: AA spent 10$ for BB. So one transaction "BB gives 10$ to AA" is needed to tally the expense.</p>
<p>Case 2: A spent 100$ for BB, BB spent 100$ for AA and AA spent 100$ for A. In this case, no transactions are required as the expenses are already tallied.</p>
<p><strong>Note:</strong> Note that A can spend for B at many places.</p>