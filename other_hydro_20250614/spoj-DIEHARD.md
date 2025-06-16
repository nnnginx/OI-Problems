<p><strong>Problem Statement:</strong></p>
<p><img src="./22146/file/auDMvztU.png" alt="" width="346" height="332"></p>

<p>The game is simple. You initially have ¡®H¡¯ amount of health and ¡®A¡¯ amount of armor. At any instant you can live in any of the three places - fire, water and air. After every unit time, you have to change your place of living. For example if you are currently living at fire, you can either step into water or air.</p>
<p>If you step into air, your health increases by 3 and your armor increases by 2</p>
<p>If you step into water, your health decreases by 5 and your armor decreases by 10</p>
<p>If you step into fire, your health decreases by 20 and your armor increases by 5</p>
<p>If your health or armor becomes &lt;=0, you will die instantly</p>
<p>Find the maximum time you can survive.</p>
<p><strong>Input:</strong></p>
<p>The first line consists of an integer t, the number of test cases. For each test case there will be two positive integers representing the initial health H and initial armor A.</p>
<p><br> <strong>Output:</strong><br><br> For each test case find the maximum time you can survive.<br><br> <strong>&nbsp;</strong></p>
<p><strong>Note:</strong> You can choose any of the 3 places during your first move.</p>
<p>&nbsp;</p>
<p><strong>Input Constraints:</strong><br><br> 1 &lt;= t &lt;= 10<br> 1 &lt;= H, A &lt;= 1000 <br><br> <strong>Example:</strong></p>

<p><strong>Sample Input:</strong></p>
<pre>3
2 10
4 4
20 8</pre>

<p><strong>Sample Output:</strong></p>
<pre>1
1
5</pre>