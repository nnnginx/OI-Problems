<p>
Canmuu is out for revenge after being utterly defeated by Bessie in paintball and has challenged Bessie to a video game.
</p>
<p>
In this game, Bessie starts out at point (BX, BY) in the coordinate grid (-1,000 &lt;= BX &lt;= 1,000; -1000 &lt;= BY &lt;= 1,000), and tries to escape, starting at time 0. She moves continuously at a velocity of (BVX, BVY) units/second (-100 &lt;= BVX &lt;= 100; -100 &lt;= BVY &lt;= 100). Thus, at time 1 she will be at point (BX + BVX, BY + BVY); at time
1.5 she will be at (BX + 1.5*BVX, BY + 1.5*BVY).
</p>
<p>
Unfortunately, Canmuu has sent N (1 &lt;= N &lt;= 50,000) cattle bruisers to pursue Bessie.  At time t=0, cattle bruiser i is at position (X_i, Y_i) (-1,000 &lt;= X_i &lt;= 1,000; -1,000 &lt;= Y_i &lt;= 1,000) with velocity (VX_i, VY_i) units/second (-1,000 &lt;= VX_i &lt;= 1,000; -1,000 &lt;= VY_i &lt;= 1,000).
</p>
<p>
Each cattle bruiser carries a "proximity" weapon to fire at Bessie; the weapon can hurt Bessie when the cattle bruiser is no further than R (1 &lt;= R &lt;= 2,500) units from her.
</p>
<p>
Bessie has a shield to protect herself from these attacks. However, she does not want to waste any of her shield's power, so she would like to know the maximum number of cattle bruisers within firing range for any (potentially non-integer) time t &gt;= 0.
</p>
<p>
In order to avoid precision errors with real numbers, it is guaranteed that the answer produced will be the same whether the attack range is decreased to R-0.0001 or increased to R+0.0001.
</p>
<h3>Input</h3>
<p>

* Line 1: Six space-separated integers: N, R, BX, BY, BVX, and BVY

* Lines 2..N+1: Line i+1 contains four space-separated integers: X_i,
        Y_i, VX_i, and VY_i

</p><h3>Output</h3>
<p>

* Line 1: Print a single integer denoting the maximum number of cattle
        bruisers within attack range at any point in time.
</p><h3>Example</h3>

<pre><b>Input:</b>

3 1 0 0 0 2
0 -3 0 4
1 2 -1 1
1 -2 2 -1
</pre>

<b>Input details:</b>
<p>
Bessie starts at point (0, 0) and is moving at 2 units per second in the (positive) y-direction. There are 3 cattle bruisers, the first of which starts at point (0, -3) and travels 4 units per second in the y-direction. The maximum distance for a cattle bruiser to be in range of Bessie is 1 unit.
</p>
<pre><b>Output:</b>

2
</pre>
<b>Output details:</b>
<p>
At time 1.5, Bessie is at point (0, 3), and the three bruisers are at points (0, 3), (-0.5, 3.5), and (4, -3.5). The first two cattle bruisers are within 1 unit of Bessie, while the third will never be within 1 unit of Bessie, so 2 is the most achievable.
</p>