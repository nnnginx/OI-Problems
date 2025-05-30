## Description

<div><p>You are playing another computer game, and now you have to slay $n$ monsters. These monsters are standing in a circle, numbered clockwise from $1$ to $n$. Initially, the $i$-th monster has $a_i$ health.</p><p>You may shoot the monsters to kill them. Each shot requires exactly one bullet and decreases the health of the targeted monster by $1$ (deals $1$ damage to it). Furthermore, when the health of some monster $i$ becomes $0$ or less than $0$, it dies and explodes, dealing $b_i$ damage to the next monster (monster $i + 1$, if $i &lt; n$, or monster $1$, if $i = n$). If the next monster is already dead, then nothing happens. If the explosion kills the next monster, it explodes too, damaging the monster after it and possibly triggering another explosion, and so on.</p><p>You have to calculate the minimum number of bullets you have to fire to kill all $n$ monsters in the circle.</p></div><div class="input-specification"><p>The first line contains one integer $T$ ($1 \le T \le 150000$) ！ the number of test cases.</p><p>Then the test cases follow, each test case begins with a line containing one integer $n$ ($2 \le n \le 300000$) ！ the number of monsters. Then $n$ lines follow, each containing two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le 10^{12}$) ！ the parameters of the $i$-th monster in the circle.</p><p>It is guaranteed that the total number of monsters in all test cases does not exceed $300000$.</p></div><div class="output-specification"><p>For each test case, print one integer ！ the minimum number of bullets you have to fire to kill all of the monsters.</p></div>

## Input

<p>The first line contains one integer $T$ ($1 \le T \le 150000$) ！ the number of test cases.</p><p>Then the test cases follow, each test case begins with a line containing one integer $n$ ($2 \le n \le 300000$) ！ the number of monsters. Then $n$ lines follow, each containing two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le 10^{12}$) ！ the parameters of the $i$-th monster in the circle.</p><p>It is guaranteed that the total number of monsters in all test cases does not exceed $300000$.</p>

## Output

<p>For each test case, print one integer ！ the minimum number of bullets you have to fire to kill all of the monsters.</p>

## Samples

```input1
1
3
7 15
2 14
5 3
```

```output1
6
```



