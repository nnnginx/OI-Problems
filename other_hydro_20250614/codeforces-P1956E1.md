## Description

<div><p><span class="tex-font-style-it">This is the easy version of the problem. The only difference between the versions is the constraints on $a_i$. You can make hacks only if both versions of the problem are solved.</span></p><p>Nene is fighting with $n$ monsters, located in a circle. These monsters are numbered from $1$ to $n$, and the $i$-th ($1 \le i \le n$) monster's current energy level is $a_i$.</p><p>Since the monsters are too strong, Nene decided to fight with them using the <span class="tex-font-style-tt">Attack Your Neighbour</span> spell. When Nene uses this spell, the following actions happen in the following order <span class="tex-font-style-bf">one by one</span>: </p><ul> <li> The $1$-st monster attacks the $2$-nd monster; </li><li> The $2$-nd monster attacks the $3$-rd monster; </li><li> $\ldots$ </li><li> The $(n-1)$-th monster attacks the $n$-th monster; </li><li> The $n$-th monster attacks the $1$-st monster. </li></ul><p>When the monster with energy level $x$ attacks the monster with the energy level $y$, the energy level of the defending monster becomes $\max(0, y-x)$ (the energy level of the attacking monster remains equal to $x$).</p><p>Nene is going to use this spell $10^{100}$ times and deal with the monsters that will still have a non-zero energy level herself. She wants you to determine which monsters will have a non-zero energy level once she will use the described spell $10^{100}$ times.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of test cases follows.</p><p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of monsters.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 2 \cdot 10^5$)&nbsp;！ the current energy levels of monsters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, </p><ul> <li> in the first line output an integer $m$&nbsp;！ the number of monsters with non-zero energy level after $10^{100}$ uses of the spell; </li><li> in the second line of output $m$ integers $i_1,i_2,\ldots,i_m$ ($1 \le i_1 &lt; i_2 &lt; \ldots &lt; i_m \le n$)&nbsp;！ the indices of these monsters in the increasing order. </li></ul><p>If $m=0$, you may either output an empty line or don't output it.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of test cases follows.</p><p>The first line contains a single integer $n$ ($2 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of monsters.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 2 \cdot 10^5$)&nbsp;！ the current energy levels of monsters.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, </p><ul> <li> in the first line output an integer $m$&nbsp;！ the number of monsters with non-zero energy level after $10^{100}$ uses of the spell; </li><li> in the second line of output $m$ integers $i_1,i_2,\ldots,i_m$ ($1 \le i_1 &lt; i_2 &lt; \ldots &lt; i_m \le n$)&nbsp;！ the indices of these monsters in the increasing order. </li></ul><p>If $m=0$, you may either output an empty line or don't output it.</p>





```input1|2,3,6,7,10,11
5
3
2 5 3
2
0 0
4
1 5 7 2
4
4 2 1 2
13
1 1 4 5 1 4 1 9 1 9 8 1 0
```




```output1
1
1 
0

1
1 
2
1 3 
6
1 3 6 8 10 12
```



## Note

<p>In the first test case, the following actions happen during the first $3$ uses of the spell in this order:</p><ul> <li> Nene uses the <span class="tex-font-style-tt">Attack Your Neighbour</span> spell for the first time; </li><li> the $1$-st monster attacks the $2$-nd monster, after the attack the energy level of the $2$-nd monster becomes equal to $\max(0, 5-2)=3$; </li><li> the $2$-nd monster attacks the $3$-rd monster, after the attack the energy level of the $3$-rd monster becomes equal to $\max(0, 3-3)=0$; </li><li> the $3$-rd monster attacks the $1$-st monster, after the attack the energy level of the $1$-st monster becomes equal to $\max(0, 2-0)=2$; </li><li> Nene uses the <span class="tex-font-style-tt">Attack Your Neighbour</span> spell for the second time; </li><li> the $1$-st monster attacks the $2$-nd monster, after the attack the energy level of the $2$-nd monster becomes equal to $\max(0, 3-2)=1$; </li><li> the $2$-nd monster attacks the $3$-rd monster, after the attack the energy level of the $3$-rd monster becomes equal to $\max(0, 0-1)=0$; </li><li> the $3$-rd monster attacks the $1$-st monster, after the attack the energy level of the $1$-st monster becomes equal to $\max(0, 2-0)=2$; </li><li> Nene uses the <span class="tex-font-style-tt">Attack Your Neighbour</span> spell for the third time; </li><li> the $1$-st monster attacks the $2$-nd monster, after the attack the energy level of the $2$-nd monster becomes equal to $\max(0, 1-2)=0$; </li><li> the $2$-nd monster attacks the $3$-rd monster, after the attack the energy level of the $3$-rd monster becomes equal to $\max(0, 0-0)=0$; </li><li> the $3$-rd monster attacks the $1$-st monster, after the attack the energy level of the $1$-st monster becomes equal to $\max(0, 2-0)=2$. </li></ul><p>After each of the next uses of the spell, energy levels of monsters do not change. Thus, only the $1$-st monster has a non-zero energy level in the end.</p><p>In the second test case, both monsters initially have zero energy level.</p>
