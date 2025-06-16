<p>Being a big foodie Golu wants to try all the dishes available at a party but because of his increasing weight his mother does not allow him to do so. After a huge fight they both come to an agreement.</p>
<p>1.&nbsp; The first rule of the agreement says that Golu should only eat at an interval of 10 minutes.</p>
<p>2.&nbsp; The second rule is regarding the stalls available. There are N stalls in one line and Golu should select only one stall to eat at one time. The selected stall must lie at the n/2th position or (n/2 + 1) position (zero indexed) among all remaining stalls.</p>
<p>3.&nbsp; Once he has selected a stall he must discard all the stalls to its left (or right) and in future can only eat from the remaining stalls. Also he can eat from a stall only once during the party, so once he has eaten from a stall, it should be discarded too.</p>
<p>The initial cooking speed at all the stalls is 1 unit. After doing some calculations Golu realises that the speed of cooking of the cook at every stall becomes double every 10 minutes. Depending upon the type of dish available and his eating capacity, he assigned a value to each stall such that any point of time he can eat a quantity which is equal to (value of that stall) * (current speed of cooking at that stall). Since speed is increasing exponentially he only remembers speed as speed % mod at any time.</p>
<p>Since he wants to eat the maximum amount of food, help him in developing a strategy to eat.</p>
<p><strong> NOTE: If there are only 2 stalls left, he must choose any one stall and discard the other.</strong></p>
<h3>Input</h3>
<p>First line contains T, the number of test cases. (1&lt;=T&lt;=5)</p>
<p>First line of each test case contains n, the number of stalls in the party. (1&lt;=n&lt;=3000)</p>
<p>Next line of each test case contains n space separated integers, representing the value of each of the stalls. (All values are between 1 and 3000 inclusive)</p>
<h3>Output</h3>
<p>Output T lines, one for each test case containing the maximum amount of food Golu can eat mod 10^9+7</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>1</p><p>5</p><p>2 4 1 3 5</p>
<strong>Output:</strong>
21</pre>
<pre><strong>Explanation:</strong></pre>
<p>Golu can select the fourth stall first and discard all stalls to its right (i.e discard fifth stall). Then he can select the third stall and again discard all stalls to its right (no stall to discard this time). Finally he chooses the 2<sup>nd</sup> stall.Therefore total food he can eat = 3*1 + 1*2 + 4*4 = 21.</p>