<p>Sabbir is a little boy. he went to a gift shop with his mother. there were&nbsp;<strong>n </strong>different types of gifts in the shop . all gifts were attractive to sabbir. he wanted to buy all the gifts which are in price range &nbsp;<a href="https://www.codecogs.com/eqnedit.php?latex=a&amp;space;\leq&amp;space;p&amp;space;\leq&amp;space;b" target="_blank"><img title="a \leq p \leq b" src="./24316/file/gPNkaSFh.png" alt=""></a>&nbsp; . you are given prices of all the gifts and &nbsp;<strong>a </strong>,&nbsp;<strong>b </strong>. sabbir's mother need your help. &nbsp;please calculate the total amount of price of all gifts of that range for sabbir's mother.&nbsp;</p>
<h3>Input</h3>
<p>in the first line there will be&nbsp;<strong>n . </strong>number of gifts in the shop.<br>in the next line there will be <strong>n&nbsp;</strong>integers <strong>p</strong><sub>1</sub><strong>, p</strong><sub>2 </sub><strong>, p</strong><sub>3 </sub><strong>... p</strong><sub><strong><sub>n &nbsp;&nbsp;</sub></strong></sub>denoting&nbsp;price of every gift</p>
<p><span style="vertical-align: sub;">in the 3rd line there will be <strong>Q</strong></span><strong>&nbsp;</strong><span style="vertical-align: sub;">number of queries.</span></p>
<p><span style="vertical-align: sub;">next <strong>Q</strong>&nbsp;lines contain two integes <strong>a</strong> and <strong>b<br>&nbsp;</strong></span></p>
<p><a href="https://www.codecogs.com/eqnedit.php?latex=1&amp;space;\leq&amp;space;n&amp;space;\leq&amp;space;10^{5}" target="_blank"><img title="1 \leq n \leq 10^{5}" src="./24316/file/Dp6xUWSV.png" alt=""></a></p>
<p><a href="https://www.codecogs.com/eqnedit.php?latex=1&amp;space;\leq&amp;space;n&amp;space;\leq&amp;space;10^{5}" target="_blank"></a> <a href="https://www.codecogs.com/eqnedit.php?latex=1&amp;space;\leq&amp;space;p_{i}&amp;space;\leq&amp;space;10^{9}" target="_blank"><img title="1 \leq p_{i} \leq 10^{9}" src="./24316/file/BvDST1dU.png" alt=""></a></p>
<p><a href="https://www.codecogs.com/eqnedit.php?latex=1&amp;space;\leq&amp;space;p_{i}&amp;space;\leq&amp;space;10^{9}" target="_blank"></a> <a href="https://www.codecogs.com/eqnedit.php?latex=1&amp;space;\leq&amp;space;Q&amp;space;\leq&amp;space;10^{5}" target="_blank"><img title="1 \leq Q \leq 10^{5}" src="./24316/file/88U4dPot.png" alt=""></a></p>
<p><a href="https://www.codecogs.com/eqnedit.php?latex=1&amp;space;\leq&amp;space;a,b&amp;space;\leq&amp;space;10^{9}" target="_blank"><img title="1 \leq a,b \leq 10^{9}" src="./24316/file/aEksIDgY.png" alt=""></a></p>
<h3>Output</h3>
<p>print <strong>Q </strong>lines . every line contains one integer , sum of all prices for that range given in the query.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7<br>1 3 2 1 5 2 2<br>4<br>1 2<br>1 5<br>3 5<br>4 5

<strong>Output:</strong>
8<br>16<br>8<br>5<br><br><strong><span style="font-size: small;">NOTE: for first query sabbir will buy all the gifts of prices 1 , 2 , 1 , 2, 2 . so, sum is 8<br></span></strong><strong><span style="font-size: small;">for second query sabbir will buy all the gifts . so the sum is 16</span></strong><br>&nbsp;</pre>