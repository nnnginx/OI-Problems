<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Evil Doctor D has captured Hulk and put him into an underground tunnel system. The tunnel system is closed but sadly Hulk is not aware of this fact.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Tunnel structure is of the form of a asterix. There are many tunnels coming out of single center point. Hulk is left unconscious at the outer end of tunnel. Once Hulk gets up he just wants to get out of this underground system. Since its completely dark down there, Hulk adopts the following strategy : He runs to get to the center and once he gets there he randomly enters another tunnel other than the one he came from. He will run to outer end of this tunnel, come back to center and again choose a random tunnel other than presently exited one ( may as well be the first chosen one).&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You have to find out the the expected length of Hulk's path in which he would have visited the ends of all tunnels atleast once.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input :&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">First line contains integer n giving number of testcases.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">n testcases follow.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For each testcase contains k followed k space seperated integers representing the lengths of the k tunnels.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">One line per testcase containing one integer E which is the expected length of Hulk's path</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 &lt;= k &lt;= 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each integer a[i] : 1 &lt;= a[i] &lt;= 10^5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Example :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 40 40</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 50 50 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">80.0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">300.0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In testcase 1 there are two tunnels of length 40 each meeting at the center. Hulk runs from end of first to center. He will take the second on to reach the end of second. Hence 40 + 40 = 80.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In testcase 2 there are three tunnels of length 50 each meeting at the center. Hulk would run from end of 0th tunnel to center (Total: 50). Run to end of one of the other two tunnels and back to center (Total: 50 + 50*2). &nbsp;Now to cover last tunnel remaining, he either choose the third tunnel immediately with probablity 1/2 or chooses the first, goes to end, comes back to center and chooses third with probablity 1/2 * 1/2 and so on. Total expected path length = 150 + 50 * 1/2 + 150 * 1/2 * 1/2 + 250 * (1/2)^3 ..... = 300.0</div>
<p>&nbsp;</p>
<p>Evil Doctor D has captured Hulk and put him into an underground tunnel system. The tunnel system is closed but sadly Hulk is not aware of this fact.&nbsp;</p>
<p>&nbsp;</p>
<p>Tunnel structure is of the form of a asterix. There are many tunnels coming out of single center point. Hulk is left unconscious at the outer end of tunnel. Once Hulk gets up he just wants to get out of this underground system. Since its completely dark down there, Hulk adopts the following strategy : He runs to get to the center and once he gets there he randomly enters another tunnel other than the one he came from. He will run to outer end of this tunnel, come back to center and again choose a random tunnel other than presently exited one ( may as well be the first chosen one).&nbsp;</p>
<p>Note: The statring point of Hulk is at the end of the tunnel whose length is mentioned first in the array</p>
<p>You have to find out the the expected length of Hulk's path in which he would have visited the ends of all tunnels atleast once.</p>
<p>&nbsp;</p>
<p>Input :&nbsp;</p>
<p>First line contains integer n giving number of testcases.&nbsp;</p>
<p>n testcases follow.&nbsp;</p>
<p>For each testcase contains k followed k space seperated integers representing the lengths of the k tunnels.</p>
<p>&nbsp;</p>
<p>Output:</p>
<p>One line per testcase containing one number E which is the expected length of Hulk's path</p>
<p>&nbsp;</p>
<p>Constraints:</p>
<p>2 &lt;= k &lt;= 50</p>
<p>Each integer a[i] : 1 &lt;= a[i] &lt;= 10^5</p>
<p>&nbsp;</p>
<p>Example :</p>
<p>&nbsp;</p>
<p>Input:</p>
<p>2</p>
<p>2 40 40</p>
<p>3 50 50 50</p>
<p>&nbsp;</p>
<p>Output:</p>
<p>80.0</p>
<p>300.0</p>
<p>&nbsp;</p>
<p>In testcase 1 there are two tunnels of length 40 each meeting at the center. Hulk runs from end of first to center. He will take the second on to reach the end of second. Hence 40 + 40 = 80.</p>
<p>In testcase 2 there are three tunnels of length 50 each meeting at the center. Hulk would run from end of 0th tunnel to center (Total: 50). Run to end of one of the other two tunnels and back to center (Total: 50 + 50*2). &nbsp;Now to cover last tunnel remaining, he either choose the third tunnel immediately with probablity 1/2 or chooses the first, goes to end, comes back to center and chooses third with probablity 1/2 * 1/2 and so on. Total expected path length = 150 + 50 * 1/2 + 150 * 1/2 * 1/2 + 250 * (1/2)^3 ..... = 300.0</p>
<p>&nbsp;</p>
<p>&nbsp;</p>