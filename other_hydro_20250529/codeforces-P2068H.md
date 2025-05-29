## Description

<div><p>The mayor of a city wants to place $n$ statues at intersections around the city. The intersections in the city are at all points $(x, y)$ with integer coordinates. Distances between intersections are measured using Manhattan distance, defined as follows: $$ \text{distance}((x_1, y_1), (x_2, y_2)) = |x_1 - x_2| + |y_1 - y_2|. $$</p><p>The city council has provided the following requirements for the placement of the statues: </p><ul> <li> The first statue is placed at $(0, 0)$; </li><li> The $n$-th statue is placed at $(a, b)$; </li><li> For $i = 1, \dots, n-1$, the distance between the $i$-th statue and the $(i+1)$-th statue is $d_i$. </li></ul><p>It is allowed to place multiple statues at the same intersection.</p><p>Help the mayor find a valid arrangement of the $n$ statues, or determine that it does not exist.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($3 \le n \le 50$) ！ the number of statues.</p><p>The second line contains two integers $a$ and $b$ ($0 \le a, b \le 10^9$) ！ the coordinates of the intersection where the $n$-th statue must be placed.</p><p>The third line contains $n-1$ integers $d_1, \dots, d_{n-1}$ ($0 \le d_i \le 10^9$) ！ the distance between the $i$-th statue and the $(i+1)$-th statue.</p></div><div class="output-specification"><p>Print $\texttt{YES}$ if there is a valid arrangement of the $n$ statues. Otherwise, print $\texttt{NO}$.</p><p>If there is a valid arrangement, print a valid arrangement in the following $n$ lines. The $i$-th of these lines must contain two integers $x_i$ and $y_i$ ！ the coordinates of the intersection where the $i$-th statue is placed. You can print any valid arrangement if multiple exist.</p></div>

## Input

<p>The first line contains an integer $n$ ($3 \le n \le 50$) ！ the number of statues.</p><p>The second line contains two integers $a$ and $b$ ($0 \le a, b \le 10^9$) ！ the coordinates of the intersection where the $n$-th statue must be placed.</p><p>The third line contains $n-1$ integers $d_1, \dots, d_{n-1}$ ($0 \le d_i \le 10^9$) ！ the distance between the $i$-th statue and the $(i+1)$-th statue.</p>

## Output

<p>Print $\texttt{YES}$ if there is a valid arrangement of the $n$ statues. Otherwise, print $\texttt{NO}$.</p><p>If there is a valid arrangement, print a valid arrangement in the following $n$ lines. The $i$-th of these lines must contain two integers $x_i$ and $y_i$ ！ the coordinates of the intersection where the $i$-th statue is placed. You can print any valid arrangement if multiple exist.</p>





```input1|
3
5 8
9 0
```




```input2|
4
10 6
7 8 5
```




```output1
NO
```




```output2
YES
0 0
6 -1
11 2
10 6
```



## Note

<p>In the <span class="tex-font-style-bf">first sample</span>, there is no valid arrangement of the 3 statues.</p><p>In the <span class="tex-font-style-bf">second sample</span>, the sample output is shown in the following picture. Note that this is not the only valid arrangement of the 4 statues. </p><center> <img class="tex-graphics" src="./36055/file/CObc4AhI.png" style="max-width: 100.0%;max-height: 100.0%;" width="531px"> </center>
