## Description

<div><p>There are $n$ warriors in a row. The power of the $i$-th warrior is $a_i$. All powers are pairwise distinct.</p><p>You have two types of spells which you may cast: </p><ol> <li> Fireball: you spend $x$ mana and destroy <span class="tex-font-style-bf">exactly</span> $k$ consecutive warriors; </li><li> Berserk: you spend $y$ mana, choose two consecutive warriors, and the warrior with greater power destroys the warrior with smaller power. </li></ol><p>For example, let the powers of warriors be $[2, 3, 7, 8, 11, 5, 4]$, and $k = 3$. If you cast Berserk on warriors with powers $8$ and $11$, the resulting sequence of powers becomes $[2, 3, 7, 11, 5, 4]$. Then, for example, if you cast Fireball on consecutive warriors with powers $[7, 11, 5]$, the resulting sequence of powers becomes $[2, 3, 4]$.</p><p>You want to turn the current sequence of warriors powers $a_1, a_2, \dots, a_n$ into $b_1, b_2, \dots, b_m$. Calculate the minimum amount of mana you need to spend on it.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$)&nbsp;�� the length of sequence $a$ and the length of sequence $b$ respectively.</p><p>The second line contains three integers $x, k, y$ ($1 \le x, y, \le 10^9; 1 \le k \le n$)&nbsp;�� the cost of fireball, the range of fireball and the cost of berserk respectively.</p><p>The third line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$). It is guaranteed that all integers $a_i$ are pairwise distinct.</p><p>The fourth line contains $m$ integers $b_1, b_2, \dots, b_m$ ($1 \le b_i \le n$). It is guaranteed that all integers $b_i$ are pairwise distinct.</p></div><div class="output-specification"><p>Print the minimum amount of mana for turning the sequnce $a_1, a_2, \dots, a_n$ into $b_1, b_2, \dots, b_m$, or $-1$ if it is impossible.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$)&nbsp;�� the length of sequence $a$ and the length of sequence $b$ respectively.</p><p>The second line contains three integers $x, k, y$ ($1 \le x, y, \le 10^9; 1 \le k \le n$)&nbsp;�� the cost of fireball, the range of fireball and the cost of berserk respectively.</p><p>The third line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$). It is guaranteed that all integers $a_i$ are pairwise distinct.</p><p>The fourth line contains $m$ integers $b_1, b_2, \dots, b_m$ ($1 \le b_i \le n$). It is guaranteed that all integers $b_i$ are pairwise distinct.</p>

## Output

<p>Print the minimum amount of mana for turning the sequnce $a_1, a_2, \dots, a_n$ into $b_1, b_2, \dots, b_m$, or $-1$ if it is impossible.</p>

## Samples

```input1
5 2
5 2 3
3 1 4 5 2
3 5
```

```output1
8
```






```input2
4 4
5 1 4
4 3 1 2
2 4 3 1
```

```output2
-1
```






```input3
4 4
2 1 11
1 3 2 4
1 3 2 4
```

```output3
0
```



