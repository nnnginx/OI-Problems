## Description

<div><p>Codefortia is a small island country located somewhere in the West Pacific. It consists of $n$ settlements connected by $m$ bidirectional gravel roads. Curiously enough, the beliefs of the inhabitants require the time needed to pass each road to be equal either to $a$ or $b$ seconds. It's guaranteed that one can go between any pair of settlements by following a sequence of roads.</p><p>Codefortia was recently struck by the financial crisis. Therefore, the king decided to abandon some of the roads so that:</p><ul> <li> it will be possible to travel between each pair of cities using the remaining roads only, </li><li> the sum of times required to pass each remaining road will be minimum possible (in other words, remaining roads must form minimum spanning tree, using the time to pass the road as its weight), </li><li> among all the plans minimizing the sum of times above, the time required to travel between the king's residence (in settlement $1$) and the parliament house (in settlement $p$) using the remaining roads only will be minimum possible. </li></ul><p>The king, however, forgot where the parliament house was. For each settlement $p = 1, 2, \dots, n$, can you tell what is the minimum time required to travel between the king's residence and the parliament house (located in settlement $p$) after some roads are abandoned?</p></div><div class="input-specification"><p>The first line of the input contains four integers $n$, $m$, $a$ and $b$ ($2 \leq n \leq 70$, $n - 1 \leq m \leq 200$, $1 \leq a &lt; b \leq 10^7$) �� the number of settlements and gravel roads in Codefortia, and two possible travel times. Each of the following lines contains three integers $u, v, c$ ($1 \leq u, v \leq n$, $u \neq v$, $c \in \{a, b\}$) denoting a single gravel road between the settlements $u$ and $v$, which requires $c$ minutes to travel.</p><p>You can assume that the road network is connected and has no loops or multiedges.</p></div><div class="output-specification"><p>Output a single line containing $n$ integers. The $p$-th of them should denote the minimum possible time required to travel from $1$ to $p$ after the selected roads are abandoned. Note that for each $p$ you can abandon a different set of roads.</p></div>

## Input

<p>The first line of the input contains four integers $n$, $m$, $a$ and $b$ ($2 \leq n \leq 70$, $n - 1 \leq m \leq 200$, $1 \leq a &lt; b \leq 10^7$) �� the number of settlements and gravel roads in Codefortia, and two possible travel times. Each of the following lines contains three integers $u, v, c$ ($1 \leq u, v \leq n$, $u \neq v$, $c \in \{a, b\}$) denoting a single gravel road between the settlements $u$ and $v$, which requires $c$ minutes to travel.</p><p>You can assume that the road network is connected and has no loops or multiedges.</p>

## Output

<p>Output a single line containing $n$ integers. The $p$-th of them should denote the minimum possible time required to travel from $1$ to $p$ after the selected roads are abandoned. Note that for each $p$ you can abandon a different set of roads.</p>

## Samples

```input1
5 5 20 25
1 2 25
2 3 25
3 4 20
4 5 20
5 1 20
```

```output1
0 25 60 40 20
```






```input2
6 7 13 22
1 2 13
2 3 13
1 4 22
3 4 13
4 5 13
5 6 13
6 1 13
```

```output2
0 13 26 39 26 13
```




## Note

<p>The minimum possible sum of times required to pass each road in the first example is $85$ �� exactly one of the roads with passing time $25$ must be abandoned. Note that after one of these roads is abandoned, it's now impossible to travel between settlements $1$ and $3$ in time $50$.</p>
