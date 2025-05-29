<p><img title="RaceTrack" src="./23936/file/jnPhzUmu.png" alt="Car with Powers race track" width="764" height="291"></p>
<p>The race track is a straight line with starting point at Track[0] and ending point at Track[n-1]. The car is initially at Track[0].</p>
<p>Track[i]='#' if the track has a wall at Track[i].</p>
<p>The car can move from Track[i] to Track[i+1] if and only if Track[i+1] is not a wall. The time taken to move from Track[i] to Track[i+1] is 1 unit.</p>
<p>If there is a wall at Track[i+1], you can shoot it from Track[i] if you have enough bullets in the car. Once a bullet is fired, the bullets count will decrease by 1. The time required to fire a bullet is 0.</p>
<p>It is also allowed to ride the car off the track. It's allowed to move from Track[i] to offTrack[i], from offTrack[i] to offTrack[i+1] and from offTrack[i] to Track[i] (if Track[i] is not a wall). The time taken for any of these steps is 2 units.<br></p>
<p>Find the fastest possible time to finish the race. Print "Impossible" if it's impossible to finish the race.<br></p>
<p><strong>Input:</strong></p>
<p>The first line consists of an integer t, the number of test cases. For each test case, the first line consists of two integers the length of race track n and the number of bullets the car can fire followed by a line with a string representing the Track. <br></p>
<p><strong>Output:</strong></p>
<p>For each test case, print the expected result as specified in the problem statement. <br></p>
<p><strong>Input Constraints:</strong></p>
<p>1 &lt;= t &lt;= 100</p>
<p>2 &lt;= n &lt;= 1000</p>
<p>0 &lt;= bullets &lt;= 1000</p>
<p>Track[i] ¡Ê {'S','E', '0', '#'}</p>
<p>Track[0]='S', Track[n-1]='E' <br></p>
<p><strong>Sample Input:</strong></p>
<pre>10
7 3
S00000E
2 2
SE
4 1
S00E
8 1
S0000##E
8 3
S0#00#0E
7 2
S0#0##E
10 4
S00#0#0##E
5 2
S000E
7 1
S0##00E
9 0
S0000##0E
</pre>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<pre>6
1
3
13
7
12
9
4
12
15</pre>
<p>&nbsp;</p>