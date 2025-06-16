<p>Blue Mary invents a game with toy bricks. The player has N cuboids numbered from 1 to N.</p>
<p>The rule of the game is discribed below:</p>
<div align="justify">
       <ul>
               <li>
               Choose some cuboids among the N cuboids, and divide them into M(1 &lt;= M &lt;= N) piles,named them Pile<sub>1</sub>,Pile<sub>2</sub> ... Pile<sub>M</sub>. There are at least 1 cuboid in each pile. To make the game easier, for any cuboid in Pile<sub>K</sub>,its id should greater than any one in Pile<sub>K+1</sub> (1 &lt;= K &lt; M).
               </li><li>
               For each pile of cuboids,the player will put them as a tower, and he should follow the two rules below:
               </li><li>
	        The up surface of each cuboid is touched and only touched another down surface. Luckily,to make the pile looking like a tower,the up surface of the lower cuboid should cover the down surface of the higher cuboid,i.e. the length of the lower up surface is not less than that of the higher down surface, and also to the width.
               </li><li>
               In each pile,the lower cuboid has a less id than the higher cuboid.</li>
        </ul>
</div>
<p>Your task is to find a method,to make the sum of the height of each pile maximum.</p>
<h3>Input</h3>
<p>The very first line of the input contain the number t,then t cases follow.</p>
<p>For each case,The first line contain two integer number N and M. N(N&lt;=100) is the total number of the cuboids, M(M&lt;=N) is the number of the piles, separated by a single space.</p>
<p>Then N line follow, which are the description of the cuboids 1..N. Each line contains three integer numbers(&lt;=1000)- the length, width and height of that cuboid,separated by spaces.</p><p>
</p><h3>Output</h3>
<p>For each case, the output contains only one line with a single integer number - the maximum sum.</p>
<h3>Example</h3>
<pre><b><tt>Sample Input:</tt></b>
1
4 2
10 5 5
8 7 7
2 2 2
6 6 6

<b><tt>Sample Output:</tt></b>
24
</pre>