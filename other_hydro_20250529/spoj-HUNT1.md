<p>Now the hunting starts in the world named DOTA, a stupid PC game which cannot play with others together.</p>
<p>Among the individuals in the game, there are two heroes named Dwarven Sniper and Lycanthrope. Lycanthrope wants to escape from being captured; however, our Dwarven Sniper won't let him go! He will use the Silver Bullet to kill the Lycanthrope by only one shot! Yes, that's enough.</p>
<p>Lycanthrope is running on a line in the map with a constant speed. The weapon range of the Silver Bullet is limited by L meters. Dwarven Sniper can run for a while freely, and then shoot Lycanthrope. In order to show his excellent shooting skill, Dwarven Sniper wants the Silver Bullet flying as far as possible. But don't forget the flying time of the Silver Bullet due to considerable weight of the bullet. And Dwarven Sniper wants to stop the hunting as quickly as possible. So if there is more than one way to show his excellent skill, he would choose the fastest way. In this problem we consider the Silver Bullet and Lycanthrope as two points.</p>
<p>Now Dwarven Sniper wants to know the maximum length that the Silver Bullet can fly, and (under this condition) the shortest time that the hunting lasts. Specifically, the total hunting time is defined as the time interval from the start of hunting to the moment that the bullet hit Lycanthrope. Can you help him?</p>
<h3>Input</h3>
<p>There are several test cases. Each of them contains only one line which consist of 9 real numbers, that are X1, Y1, X2, Y2, Lx, Ly, vD , vB and L (-10000 &lt;= X1 , Y1 , X2 , Y2 , Lx , Ly &lt;= 10000 , 0 &lt;= vD , vB , L &lt;=100000). The pair (X1, Y1) is the starting position of the Lycanthrope while (X2, Y2) is the starting position of Dwarven Sniper, while (Lx, Ly) is the moving vector per second of the Lycanthrope, vD is the speed of the Dwarven Sniper, vB is the speed of the Silver Bullet, L is the maximum possible flying distance of the bullet.</p>
<p>All units are meters/second.</p>
<p>It is guaranteed that (Lx*Lx+Ly*Ly) &lt; vD*vD &lt; vB*vB , and Dwarven Sniper's starting position is different from Lycanthrope's position. The input ends with a line containing all zeros.</p>
<h3>Output</h3>
<p>For each test case, output two real numbers S and T in a line separated by a single space denoting that the Silver bullet flies S meters before hitting Lycanthrope and the hunting lasts for T seconds, both with 3 numbers after the decimal point.</p>
<p>You may assume that Dwarven Sniper can finish his hunting within no more than 1e+9 seconds.</p>
<p><b>Note: The judge is "ignoring extra white spaces".</b></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
-1 0 0 10 1 0 2 10 10
0 0 0 5 0 1 2 6 6
0 0 0 0 0 0 0 0 0

<strong>Output:</strong>
10.000 1.000
6.000 3.000
</pre>
<p></p>