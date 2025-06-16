<div style="font-family: verdana, geneva;">
<h1 style="text-align: center; "><strong>DOTA HEROES</strong></h1>
<p><strong>Problem Description:</strong></p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Defence Of The Ancients(DOTA) is one of the most addictive online multiplayer games. There are n heroes in our team and our motto is to conquer the opponent¡¯s empire. To safeguard their empire, the opponents had constructed m towers on the path. If one or more heroes get into the sight of a tower, then the tower does D amount of damage to one of those heroes at that instant (i.e. one of the heroes¡¯ health decreases by D). Any hero will die if his health H &lt;=0. &nbsp;Once a tower attacks one of the heroes, all the heroes in the sight of that tower at that instant get out of its sight. Find whether all of the heroes in our team can reach the opponent¡¯s empire alive.</p>
<p><strong>Input Specification:</strong></p>
<p>The first line consists of one integer t representing the number of test cases. For each test case, the first line consists of three integers n, m and D, the number of heroes, number of towers and the amount of Damage respectively. The next n lines consist of an integer representing the health of respective hero.</p>
<p><strong>Output Specification:</strong></p>
<p>Just a word ¡°<tt>YES</tt>¡± if we can reach the opponent¡¯s empire alive, else ¡°<tt>NO</tt>¡±.</p>
<p><strong>Input Constraints:</strong></p>
<p>1 &lt;= t &lt;= 500<br> 1 &lt;= n &lt;= 500<br> 1 &lt;= m &lt;= n<br> 1 &lt;= D, H &lt;= 20000</p>
<p><strong>Sample Input:</strong></p>
<pre>3
6 3 400
500
500
500
500
500
500
6 5 400
800
800
801
200
200
200<br>6 3 400<br>401<br>401<br>400<br>200<br>400<br>200</pre>
<p><strong>Sample Output:</strong></p>
<pre>YES
NO
NO</pre>
<p><strong>Explanation of test case 1:</strong></p>
<p>One of the possible solutions is <br> First, three of the heroes can goes together. One of them receives 400 damage from the first tower and all of them cross it. Then while crossing the next tower, one of the heroes who is at 500 health gets 400 damage and all of them cross it. Then the third hero receives the damage when crossing the last tower. Similarly the other 3 heroes can reach the opponent¡¯s base together without dying.</p>
</div>
<p>
<script src="data:text/javascript;base64,JCgnI3Byb2JsZW0tdGFncycpLmhpZGUoKQ=="></script>
</p>
<p>
<script src="data:text/javascript;base64,JCgnI3Byb2JsZW0tdGFncycpLmhpZGUoKQ=="></script>
</p>
<p>
<script src="data:text/javascript;base64,JCgnI3Byb2JsZW0tdGFncycpLmhpZGUoKQ=="></script>
</p>