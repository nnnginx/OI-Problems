## Description

<div><p>Recently you've discovered a new shooter. They say it has realistic game mechanics.</p><p>Your character has a gun with magazine size equal to $k$ and should exterminate $n$ waves of monsters. The $i$-th wave consists of $a_i$ monsters and happens from the $l_i$-th moment of time up to the $r_i$-th moments of time. All $a_i$ monsters spawn at moment $l_i$ and you have to exterminate all of them before the moment $r_i$ ends (you can kill monsters right at moment $r_i$). For every two consecutive waves, the second wave starts not earlier than the first wave ends (though the second wave can start at the same moment when the first wave ends) ！ formally, the condition $r_i \le l_{i + 1}$ holds. Take a look at the notes for the examples to understand the process better.</p><p>You are confident in yours and your character's skills so you can assume that aiming and shooting are instant and you need exactly one bullet to kill one monster. But reloading takes exactly $1$ unit of time.</p><p>One of the realistic mechanics is a mechanic of reloading: when you reload you throw away the old magazine with all remaining bullets in it. That's why constant reloads may cost you excessive amounts of spent bullets.</p><p>You've taken a liking to this mechanic so now you are wondering: what is the minimum possible number of bullets you need to spend (both used and thrown) to exterminate all waves.</p><p>Note that you don't throw the remaining bullets away after eradicating all monsters, and you start with a full magazine.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le n \le 2000$; $1 \le k \le 10^9$)&nbsp;！ the number of waves and magazine size.</p><p>The next $n$ lines contain descriptions of waves. The $i$-th line contains three integers $l_i$, $r_i$ and $a_i$ ($1 \le l_i \le r_i \le 10^9$; $1 \le a_i \le 10^9$)&nbsp;！ the period of time when the $i$-th wave happens and the number of monsters in it.</p><p>It's guaranteed that waves don't overlap (but may touch) and are given in the order they occur, i. e. $r_i \le l_{i + 1}$.</p></div><div class="output-specification"><p>If there is no way to clear all waves, print $-1$. Otherwise, print the minimum possible number of bullets you need to spend (both used and thrown) to clear all waves.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le n \le 2000$; $1 \le k \le 10^9$)&nbsp;！ the number of waves and magazine size.</p><p>The next $n$ lines contain descriptions of waves. The $i$-th line contains three integers $l_i$, $r_i$ and $a_i$ ($1 \le l_i \le r_i \le 10^9$; $1 \le a_i \le 10^9$)&nbsp;！ the period of time when the $i$-th wave happens and the number of monsters in it.</p><p>It's guaranteed that waves don't overlap (but may touch) and are given in the order they occur, i. e. $r_i \le l_{i + 1}$.</p>

## Output

<p>If there is no way to clear all waves, print $-1$. Otherwise, print the minimum possible number of bullets you need to spend (both used and thrown) to clear all waves.</p>

## Samples

```input1
2 3
2 3 6
3 4 3
```

```output1
9
```






```input2
2 5
3 7 11
10 12 15
```

```output2
30
```






```input3
5 42
42 42 42
42 43 42
43 44 42
44 45 42
45 45 1
```

```output3
-1
```






```input4
1 10
100 111 1
```

```output4
1
```




## Note

<p>In the first example: </p><ul> <li> At the moment $2$, the first wave occurs and $6$ monsters spawn. You kill $3$ monsters and start reloading. </li><li> At the moment $3$, the second wave occurs and $3$ more monsters spawn. You kill remaining $3$ monsters from the first wave and start reloading. </li><li> At the moment $4$, you kill remaining $3$ monsters from the second wave. </li></ul> In total, you'll spend $9$ bullets.<p>In the second example: </p><ul> <li> At moment $3$, the first wave occurs and $11$ monsters spawn. You kill $5$ monsters and start reloading. </li><li> At moment $4$, you kill $5$ more monsters and start reloading. </li><li> At moment $5$, you kill the last monster and start reloading throwing away old magazine with $4$ bullets. </li><li> At moment $10$, the second wave occurs and $15$ monsters spawn. You kill $5$ monsters and start reloading. </li><li> At moment $11$, you kill $5$ more monsters and start reloading. </li><li> At moment $12$, you kill last $5$ monsters. </li></ul> In total, you'll spend $30$ bullets.
