## Description

<div><p>Monocarp is playing a computer game. In this game, his character is a necromancer. He is fighting $n$ monsters numbered from $1$ to $n$. Each monster has two parameters: health and strength.</p><p>Monocarp considers $q$ scenarios of the battle. In each scenario, he chooses some segment $[l, r]$ of monsters and calculates the number of moves it takes to defeat all these monsters.</p><p>Each scenario proceeds as follows. First, Monocarp kills monster $l$ and revives it as a zombie (this does not count as a move). Then each move the following happens: let $i$ be the index of the first monster in the segment $[l, r]$ that is still alive. All zombies attack monster $i$, reducing its health by their total strength. After that, if monster $i$ has $0$ or less health, it dies and Monocarp revives it as a zombie.</p><p>When the monster is revived, the zombie's strength is equal to the monster's strength.</p><p>Help Monocarp for each scenario to calculate how many moves it will take to kill all the monsters in the segment.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;！ the number of monsters and the number of scenarios, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^4$), where $a_i$ is the number of health points of the $i$-th monster.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^4$), where $b_i$ is the strength of the $i$-th monster.</p><p>Then $q$ lines follow. The $j$-th of them contains two integers $l_j$ and $r_j$ ($1 \le l_j \le r_j \le n$)&nbsp;！ the boundaries of the $j$-th scenario.</p></div><div class="output-specification"><p>For each scenario, print a single integer&nbsp;！ the number of moves it will take to kill all the monsters in the segment.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;！ the number of monsters and the number of scenarios, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^4$), where $a_i$ is the number of health points of the $i$-th monster.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n$ ($1 \le b_i \le 10^4$), where $b_i$ is the strength of the $i$-th monster.</p><p>Then $q$ lines follow. The $j$-th of them contains two integers $l_j$ and $r_j$ ($1 \le l_j \le r_j \le n$)&nbsp;！ the boundaries of the $j$-th scenario.</p>

## Output

<p>For each scenario, print a single integer&nbsp;！ the number of moves it will take to kill all the monsters in the segment.</p>





```input1|
7 5
4 5 9 9 4 2 4
1 3 3 1 2 3 3
3 5
1 4
6 6
1 7
2 6
```




```output1
4
10
0
13
7
```


