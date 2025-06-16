<p style="text-align: justify;"><span style="font-size: small;">You have N marbles and K slots. You have to follow the below mentioned rules :</span></p>
<ol style="text-align: justify;">
<li><span style="font-size: small;">You can put in a marble or take out a marble from slot numbered 1 at any time.</span></li>
<li style="text-align: justify;"><span style="font-size: small;">You can put in a marble or take out a marble from slot numbered i only if there exists a marble at the slot i - 1.</span></li>
<li style="text-align: justify;"><span style="font-size: small;">The game stops when a marble reaches the slot numbered K for the first time.<br></span></li>
</ol>
<p style="text-align: justify;"><span style="font-size: small;">Your task is to finish the game in minimum number of valid moves.</span></p>
<h3 style="text-align: center;">Input</h3>
<p style="text-align: justify;"><span style="font-size: small;">The first line contains t, the number of testcases. Then on each line is given two numbers N &lt;= 15, K &lt;= 2^N - 1.<br></span></p>
<p style="text-align: justify;">&nbsp;</p>
<h3 style="text-align: center;">Output<span style="font-size: small;">&nbsp;</span></h3>
<p style="text-align: justify;"><span style="font-size: small;">Print two numbers namely the number of "put in" moves and the number of "remove from" moves respectively for all the tests such that you move to the Kth slot in minimum number of valid moves. See explanation section below for more details.<br></span></p>
<h3 style="text-align: center;">Example</h3>
<p><span style="font-size: small;"><strong>Input:</strong></span><span style="font-size: small;">&nbsp;</span></p>
<p><span style="font-size: small;">1 </span></p>
<p><span style="font-size: small;">3 6<br></span></p>
<p><span style="font-size: small;"><strong>Output:</strong></span></p>
<p><span style="font-size: small;">6 3<br></span></p>
<h3><span style="font-size: small;">Explanation :</span></h3>
<p><span style="font-size: small;">The following are the valid moves for the given input:</span></p>
<p><span style="font-size: small;">PUT IN 1<br>PUT IN 2<br>PUT IN 3<br>REMOVE FROM 2<br>REMOVE FROM 1<br>PUT IN 4<br>PUT IN 5<br>REMOVE FROM 4<br>PUT IN 6</span><span style="font-size: small;">&nbsp;</span></p>