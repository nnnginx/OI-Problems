## Description

<div><p>Palo Alto is an unusual city because it is an endless coordinate line. It is also known for the office of Lyft Level 5.</p><p>Lyft has become so popular so that it is now used by all $m$ taxi drivers in the city, who every day transport the rest of the city residents&nbsp;�� $n$ riders.</p><p>Each resident (including taxi drivers) of Palo-Alto lives in its unique location (there is no such pair of residents that their coordinates are the same).</p><p>The Lyft system is very clever: when a rider calls a taxi, his call does not go to all taxi drivers, but only to the one that is the closest to that person. If there are multiple ones with the same distance, then to taxi driver with a smaller coordinate is selected.</p><p>But one morning the taxi drivers wondered: how many riders are there that would call the given taxi driver if they were the first to order a taxi on that day? In other words, you need to find for each taxi driver $i$ the number $a_{i}$&nbsp;�� the number of riders that would call the $i$-th taxi driver when all drivers and riders are at their home?</p><p>The taxi driver can neither transport himself nor other taxi drivers.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n,m \le 10^5$)&nbsp;�� number of riders and taxi drivers.</p><p>The second line contains $n + m$ integers $x_1, x_2, \ldots, x_{n+m}$ ($1 \le x_1 &lt; x_2 &lt; \ldots &lt; x_{n+m} \le 10^9$), where $x_i$ is the coordinate where the $i$-th resident lives. </p><p>The third line contains $n + m$ integers $t_1, t_2, \ldots, t_{n+m}$ ($0 \le t_i \le 1$). If $t_i = 1$, then the $i$-th resident is a taxi driver, otherwise $t_i = 0$.</p><p>It is guaranteed that the number of $i$ such that $t_i = 1$ is equal to $m$.</p></div><div class="output-specification"><p>Print $m$ integers $a_1, a_2, \ldots, a_{m}$, where $a_i$ is the answer for the $i$-th taxi driver. The taxi driver has the number $i$ if among all the taxi drivers he lives in the $i$-th smallest coordinate (see examples for better understanding).</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n,m \le 10^5$)&nbsp;�� number of riders and taxi drivers.</p><p>The second line contains $n + m$ integers $x_1, x_2, \ldots, x_{n+m}$ ($1 \le x_1 &lt; x_2 &lt; \ldots &lt; x_{n+m} \le 10^9$), where $x_i$ is the coordinate where the $i$-th resident lives. </p><p>The third line contains $n + m$ integers $t_1, t_2, \ldots, t_{n+m}$ ($0 \le t_i \le 1$). If $t_i = 1$, then the $i$-th resident is a taxi driver, otherwise $t_i = 0$.</p><p>It is guaranteed that the number of $i$ such that $t_i = 1$ is equal to $m$.</p>

## Output

<p>Print $m$ integers $a_1, a_2, \ldots, a_{m}$, where $a_i$ is the answer for the $i$-th taxi driver. The taxi driver has the number $i$ if among all the taxi drivers he lives in the $i$-th smallest coordinate (see examples for better understanding).</p>

## Samples

```input1
3 1
1 2 3 10
0 0 1 0

```

```output1
3
```






```input2
3 2
2 3 4 5 6
1 0 0 0 1

```

```output2
2 1
```






```input3
1 4
2 4 6 10 15
1 1 1 1 0

```

```output3
0 0 0 1
```




## Note

<p>In the first example, we have only one taxi driver, which means an order from any of $n$ riders will go to him.</p><p>In the second example, the first taxi driver lives at the point with the coordinate $2$, and the second one lives at the point with the coordinate $6$. Obviously, the nearest taxi driver to the rider who lives on the $3$ coordinate is the first one, and to the rider who lives on the coordinate $5$ is the second one. The rider who lives on the $4$ coordinate has the same distance to the first and the second taxi drivers, but since the first taxi driver has a smaller coordinate, the call from this rider will go to the first taxi driver.</p><p>In the third example, we have one rider and the taxi driver nearest to him is the fourth one.</p>
