## Description

<div><p>Pelican Town represents $n$ houses connected by $m$ bidirectional roads. Some roads have <span class="tex-font-style-it">NPCs</span> standing on them. Farmer Buba needs to walk on each road with an NPC and talk to them.</p><p>Help the farmer find a route satisfying the following properties: </p><ul> <li> The route starts at some house, follows the roads, and ends at the same house. </li><li> The route does not follow any road more than once (in both directions together). </li><li> The route follows each road with an NPC exactly once. </li></ul> Note that the route can follow roads without NPCs, and you do <span class="tex-font-style-bf">not</span> need to minimize the length of the route.<p>It is <span class="tex-font-style-bf">guaranteed</span> that you can reach any house from any other by walking on the roads with NPCs only.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq 5 \cdot 10^5, 1 \leq m \leq 5 \cdot 10^5$)&nbsp;！ the number of houses and roads in <span class="tex-font-style-tt">Pelican Town</span> respectively.</p><p>In each of the next $m$ lines, three integers $u$, $v$, and $c$ ($1 \leq u, v \leq n, c = 0/1$) are given&nbsp;！ the ends of the road and whether an <span class="tex-font-style-tt">NPC</span> is on this road. If $c = 1$, then the road has an NPC. If $c = 0$, then the road has no NPC.</p><p>The graph may contain multiple edges and loops, and if there are multiple edges with <span class="tex-font-style-tt">NPCs</span> standing on them, the route must follow each of these roads.</p><p>It is guaranteed that you can reach any house from any other by walking on the roads with NPCs only.</p><p>It is guaranteed that the sum of $n$ and $m$ for all test cases does not exceed $5 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, if there is no solution, then output "<span class="tex-font-style-tt">No</span>" (without quotes). </p><p>Otherwise, output "<span class="tex-font-style-tt">Yes</span>" (without quotes), and then output $k$&nbsp;！ the number of roads in the route. In the next line, output $k + 1$ numbers&nbsp;！ the houses of the route in the order of traversal. Note that the first house should match the last one, as the route is cyclic.</p><p>If there are multiple answers, you can print any of them.</p><p>You can output each letter in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n \leq 5 \cdot 10^5, 1 \leq m \leq 5 \cdot 10^5$)&nbsp;！ the number of houses and roads in <span class="tex-font-style-tt">Pelican Town</span> respectively.</p><p>In each of the next $m$ lines, three integers $u$, $v$, and $c$ ($1 \leq u, v \leq n, c = 0/1$) are given&nbsp;！ the ends of the road and whether an <span class="tex-font-style-tt">NPC</span> is on this road. If $c = 1$, then the road has an NPC. If $c = 0$, then the road has no NPC.</p><p>The graph may contain multiple edges and loops, and if there are multiple edges with <span class="tex-font-style-tt">NPCs</span> standing on them, the route must follow each of these roads.</p><p>It is guaranteed that you can reach any house from any other by walking on the roads with NPCs only.</p><p>It is guaranteed that the sum of $n$ and $m$ for all test cases does not exceed $5 \cdot 10^5$.</p>

## Output

<p>For each test case, if there is no solution, then output "<span class="tex-font-style-tt">No</span>" (without quotes). </p><p>Otherwise, output "<span class="tex-font-style-tt">Yes</span>" (without quotes), and then output $k$&nbsp;！ the number of roads in the route. In the next line, output $k + 1$ numbers&nbsp;！ the houses of the route in the order of traversal. Note that the first house should match the last one, as the route is cyclic.</p><p>If there are multiple answers, you can print any of them.</p><p>You can output each letter in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,4,9,10,11,12,13,14,15,16,17,18
3
3 2
1 2 1
2 3 1
3 3
1 2 1
1 3 1
2 3 0
5 9
1 2 0
5 2 1
5 4 1
5 1 1
2 3 1
5 2 1
4 1 0
4 3 0
5 2 0
```




```output1
NO
YES
3
1 2 3 1 
YES
7
1 2 5 4 3 2 5 1
```



## Note

<p>Note that in the third test case, there are multiple edges $(5, 2)$. You must walk on two of them.</p>
