## Description

<div><p>There are $n$ monsters standing in a row. The $i$-th monster has $a_i$ health points.</p><p>Every second, you can choose one <span class="tex-font-style-bf">alive</span> monster and launch a chain lightning at it. The lightning deals $k$ damage to it, and also spreads to the left (towards decreasing $i$) and to the right (towards increasing $i$) to <span class="tex-font-style-bf">alive</span> monsters, dealing $k$ damage to each. When the lightning reaches a dead monster or the beginning/end of the row, it stops. A monster is considered alive if its health points are strictly greater than $0$.</p><p>For example, consider the following scenario: there are three monsters with health equal to $[5, 2, 7]$, and $k = 3$. You can kill them all in $4$ seconds:</p><ul> <li> launch a chain lightning at the $3$-rd monster, then their health values are $[2, -1, 4]$; </li><li> launch a chain lightning at the $1$-st monster, then their health values are $[-1, -1, 4]$; </li><li> launch a chain lightning at the $3$-rd monster, then their health values are $[-1, -1, 1]$; </li><li> launch a chain lightning at the $3$-th monster, then their health values are $[-1, -1, -2]$. </li></ul><p>For each $k$ from $1$ to $\max(a_1, a_2, \dots, a_n)$, calculate the minimum number of seconds it takes to kill all the monsters.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the number of monsters.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$)&nbsp;！ the health points of the $i$-th monster.</p></div><div class="output-specification"><p>For each $k$ from $1$ to $\max(a_1, a_2, \dots, a_n)$, output the minimum number of seconds it takes to kill all the monsters.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the number of monsters.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$)&nbsp;！ the health points of the $i$-th monster.</p>

## Output

<p>For each $k$ from $1$ to $\max(a_1, a_2, \dots, a_n)$, output the minimum number of seconds it takes to kill all the monsters.</p>





```input1|
3
5 2 7
```




```input2|
4
7 7 7 7
```




```input3|
10
1 9 7 6 2 4 7 8 1 3
```




```output1
10 6 4 3 2 2 1
```




```output2
7 4 3 2 2 2 1
```




```output3
17 9 5 4 3 3 3 2 1
```


