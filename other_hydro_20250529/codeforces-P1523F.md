## Description

<div><center> <img class="tex-graphics" height="378px" src="./32083/file/O9rmvXsl.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center><p>After William is done with work for the day, he enjoys playing his favorite video game.</p><p>The game happens in a 2D world, starting at turn $0$. William can pick any cell in the game world and spawn in it. Then, each turn, William may remain at his current location or move from the current location (x, y) to one of the following locations: (x + 1, y), (x - 1, y), (x, y + 1), (x, y - 1).</p><p>To accelerate movement the game has $n$ fast travel towers. $i$-th tower is located at location ($xa_i, ya_i$). To be able to instantly travel to the tower from any location in the game world it must first be activated. Activation of tower $i$ happens at the moment when the player is in cell ($xa_i, ya_i$) after this the tower remains active throughout the entire game.</p><p>William also knows that the game has $m$ quests. $i$-th quest can be completed instantly by being at location ($xb_i, yb_i$) on turn $t_i$.</p><p>William wants to find out the maximal number of quests he will be able to complete by optimally traversing the game world.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($0 \le n \le 14, 1 \le m \le 100$), which are the number of towers and the number of quests, respectively.</p><p>Each of the next $n$ lines contains two integers $xa_i, ya_i$ ($1 \le xa_i, ya_i \le 10^6$), which are the coordinates of fast travel towers.</p><p>Each of the next $m$ lines contains two integers $xb_i$, $yb_i$ and $t_i$ ($1 \le xb_i, yb_i \le 10^6$, $1 \le t_i \le 10^9$), which are the coordinates of quests and the turn at which it may be completed.</p><p>It is guaranteed that all locations in a test are different.</p></div><div class="output-specification"><p>Print a single number &nbsp;�� the maximal number of quests William will be able to complete.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($0 \le n \le 14, 1 \le m \le 100$), which are the number of towers and the number of quests, respectively.</p><p>Each of the next $n$ lines contains two integers $xa_i, ya_i$ ($1 \le xa_i, ya_i \le 10^6$), which are the coordinates of fast travel towers.</p><p>Each of the next $m$ lines contains two integers $xb_i$, $yb_i$ and $t_i$ ($1 \le xb_i, yb_i \le 10^6$, $1 \le t_i \le 10^9$), which are the coordinates of quests and the turn at which it may be completed.</p><p>It is guaranteed that all locations in a test are different.</p>

## Output

<p>Print a single number &nbsp;�� the maximal number of quests William will be able to complete.</p>

## Samples

```input1
3 4
1 1
2 3
5 2
2 2 12
5 1 4
6 2 11
3 5 10
```

```output1
3
```




## Note

<p>In the first sample test one of the possible sequences of William's actions is as follows: </p><ul> <li> Spawn at $(3, 2)$ </li><li> On turn $1$ move to $(4, 2)$ </li><li> On turn $2$ move to $(5, 2)$. By visiting this cell William activates tower number $3$. </li><li> On turn $3$ move to $(5, 1)$, where he waits for $1$ turn to complete the $2$nd quest </li><li> On turn $5$ move to $(5, 2)$ </li><li> On turn $6$ move to $(5, 3)$ </li><li> On turn $7$ move to $(5, 4)$ </li><li> On turn $8$ move to $(5, 5)$ </li><li> On turn $9$ move to $(4, 5)$ </li><li> On turn $10$ move to $(3, 5)$. By moving to this location William will complete the $4$th quest </li><li> On turn $10$ instantly move to an already activated fast travel tower at $(5, 2)$ </li><li> On turn $11$ move to $(6, 2)$. By moving to this location William will complete the $3$rd quest </li><li> William will not be able to complete the quest number $1$, because the tower at $(2, 3)$ was not activated </li></ul>
