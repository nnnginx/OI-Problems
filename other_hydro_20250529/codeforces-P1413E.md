## Description

<div><p>Meka-Naruto plays a computer game. His character has the following ability: given an enemy hero, deal $a$ instant damage to him, and then heal that enemy $b$ health points at the end of every second, for exactly $c$ seconds, starting one second after the ability is used. That means that if the ability is used at time $t$, the enemy's health decreases by $a$ at time $t$, and then increases by $b$ at time points $t + 1$, $t + 2$, ..., $t + c$ due to this ability.</p><p>The ability has a cooldown of $d$ seconds, i.&nbsp;e. if Meka-Naruto uses it at time moment $t$, next time he can use it is the time $t + d$. Please note that he can only use the ability at integer points in time, so all changes to the enemy's health also occur at integer times only.</p><p>The effects from different uses of the ability may stack with each other; that is, the enemy which is currently under $k$ spells gets $k\cdot b$ amount of heal this time. Also, if several health changes occur at the same moment, they are all counted at once.</p><p>Now Meka-Naruto wonders if he can kill the enemy by just using the ability each time he can (that is, every $d$ seconds). The enemy is killed if their health points become $0$ or less. Assume that the enemy's health is not affected in any way other than by Meka-Naruto's character ability. What is the maximal number of health points the enemy can have so that Meka-Naruto is able to kill them?</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1\leq t\leq 10^5$) standing for the number of testcases.</p><p>Each test case is described with one line containing four numbers $a$, $b$, $c$ and $d$ ($1\leq a, b, c, d\leq 10^6$) denoting the amount of instant damage, the amount of heal per second, the number of heals and the ability cooldown, respectively.</p></div><div class="output-specification"><p>For each testcase in a separate line print $-1$ if the skill can kill an enemy hero with an arbitrary number of health points, otherwise print the maximal number of health points of the enemy that can be killed.</p></div>

## Input

<p>The first line contains an integer $t$ ($1\leq t\leq 10^5$) standing for the number of testcases.</p><p>Each test case is described with one line containing four numbers $a$, $b$, $c$ and $d$ ($1\leq a, b, c, d\leq 10^6$) denoting the amount of instant damage, the amount of heal per second, the number of heals and the ability cooldown, respectively.</p>

## Output

<p>For each testcase in a separate line print $-1$ if the skill can kill an enemy hero with an arbitrary number of health points, otherwise print the maximal number of health points of the enemy that can be killed.</p>

## Samples

```input1
7
1 1 1 1
2 2 2 2
1 2 3 4
4 3 2 1
228 21 11 3
239 21 11 3
1000000 1 1000000 1
```

```output1
1
2
1
5
534
-1
500000500000
```




## Note

<p>In the first test case of the example each unit of damage is cancelled in a second, so Meka-Naruto cannot deal more than 1 damage.</p><p>In the fourth test case of the example the enemy gets:</p><ul> <li> $4$ damage ($1$-st spell cast) at time $0$; </li><li> $4$ damage ($2$-nd spell cast) and $3$ heal ($1$-st spell cast) at time $1$ (the total of $5$ damage to the initial health); </li><li> $4$ damage ($3$-nd spell cast) and $6$ heal ($1$-st and $2$-nd spell casts) at time $2$ (the total of $3$ damage to the initial health); </li><li> and so on. </li></ul><p>One can prove that there is no time where the enemy gets the total of $6$ damage or more, so the answer is $5$. Please note how the health is recalculated: for example, $8$-health enemy would <span class="tex-font-style-bf">not</span> die at time $1$, as if we first subtracted $4$ damage from his health and then considered him dead, before adding $3$ heal.</p><p>In the sixth test case an arbitrarily healthy enemy can be killed in a sufficient amount of time.</p><p>In the seventh test case the answer does not fit into a 32-bit integer type.</p>
