## Description

<div><p>Polycarp is an introvert person. In fact he is so much of an introvert that he plays "Monsters and Potions" board game alone. The board of the game is a row of $n$ cells. The cells are numbered from $1$ to $n$ from left to right. There are three types of cells: a cell containing a single monster, a cell containing a single potion or a <span class="tex-font-style-it">blank</span> cell (it contains neither a monster nor a potion).</p><p>Polycarp has $m$ tokens representing heroes fighting monsters, which are initially located in the blank cells $s_1, s_2, \dots, s_m$. Polycarp's task is to choose a single cell (rally point) and one by one move all the heroes into this cell. A rally point can be a cell of any of three types.</p><p>After Policarp selects a rally point, he picks a hero and orders him to move directly to the point. Once that hero reaches the point, Polycarp picks another hero and orders him also to go to the point. And so forth, until all the heroes reach the rally point cell. While going to the point, a hero can not deviate from the direct route or take a step back. A hero just moves cell by cell in the direction of the point until he reaches it. It is possible that multiple heroes are simultaneously in the same cell.</p><p>Initially the $i$-th hero has $h_i$ hit points (HP). Monsters also have HP, different monsters might have different HP. And potions also have HP, different potions might have different HP.</p><p>If a hero steps into a cell which is blank (i.e. doesn't contain a monster/potion), hero's HP does not change.</p><p>If a hero steps into a cell containing a monster, then the hero and the monster fight. If monster's HP is strictly higher than hero's HP, then the monster wins and Polycarp loses the whole game. If hero's HP is greater or equal to monster's HP, then the hero wins and monster's HP is subtracted from hero's HP. I.e. the hero survives if his HP drops to zero, but dies (and Polycarp looses) if his HP becomes negative due to a fight. If a hero wins a fight with a monster, then the monster disappears, and the cell becomes blank.</p><p>If a hero steps into a cell containing a potion, then the hero drinks the potion immediately. As a result, potion's HP is added to hero's HP, the potion disappears, and the cell becomes blank.</p><p>Obviously, Polycarp wants to win the game. It means that he must choose such rally point and the order in which heroes move, that every hero reaches the rally point and survives. I.e. Polycarp loses if a hero reaches rally point but is killed by a monster at the same time. Polycarp can use any of $n$ cells as a rally point ！ initially it can contain a monster, a potion, or be a blank cell with or without a hero in it.</p><p>Help Polycarp write a program to choose a rally point and the order in which heroes move.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $m$ ($1 \le n \le 100$; $1 \le m \le n$) ！ length of the game board and the number of heroes on it.</p><p>The following $m$ lines describe heroes. Each line contains two integers $s_i$ and $h_i$ ($1 \le s_i \le n$; $1 \le h_i \le 10^6$), where $s_i$ is the initial position and $h_i$ is the initial HP of the $i$-th hero. It is guaranteed that each cell $s_i$ is blank. It is also guaranteed that all $s_i$ are different. </p><p>The following line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^6 \le a_j \le 10^6$), where $a_j$ describes the $i$-th cell of the game board:</p><ul> <li> $a_j=0$ means that the $i$-th cell is blank, </li><li> $a_j&lt;0$ means that the $i$-th cell contains monster with positive HP of $-a_j$, </li><li> $a_j&gt;0$ means that the $i$-th cell contains potion with $a_j$ HP. </li></ul></div><div class="output-specification"><p>On the first line of the output print the index of the rally point cell.</p><p>On the second line print $m$ integers ！ the order in which heroes should move to the rally point. Heroes are numbered from $1$ to $m$ in the order they are given in the input.</p><p>If there are multiple solutions, print any of them.</p><p>If it is impossible to find a rally point which can be reached by all heroes, print a single integer <span class="tex-font-style-tt">-1</span> in the output.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $m$ ($1 \le n \le 100$; $1 \le m \le n$) ！ length of the game board and the number of heroes on it.</p><p>The following $m$ lines describe heroes. Each line contains two integers $s_i$ and $h_i$ ($1 \le s_i \le n$; $1 \le h_i \le 10^6$), where $s_i$ is the initial position and $h_i$ is the initial HP of the $i$-th hero. It is guaranteed that each cell $s_i$ is blank. It is also guaranteed that all $s_i$ are different. </p><p>The following line contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^6 \le a_j \le 10^6$), where $a_j$ describes the $i$-th cell of the game board:</p><ul> <li> $a_j=0$ means that the $i$-th cell is blank, </li><li> $a_j&lt;0$ means that the $i$-th cell contains monster with positive HP of $-a_j$, </li><li> $a_j&gt;0$ means that the $i$-th cell contains potion with $a_j$ HP. </li></ul>

## Output

<p>On the first line of the output print the index of the rally point cell.</p><p>On the second line print $m$ integers ！ the order in which heroes should move to the rally point. Heroes are numbered from $1$ to $m$ in the order they are given in the input.</p><p>If there are multiple solutions, print any of them.</p><p>If it is impossible to find a rally point which can be reached by all heroes, print a single integer <span class="tex-font-style-tt">-1</span> in the output.</p>

## Samples

```input1
8 3
8 2
1 3
4 9
0 3 -5 0 -5 -4 -1 0

```

```output1
6
3 1 2
```






```input2
1 1
1 1
0

```

```output2
1
1
```






```input3
3 2
1 1
3 1
0 -5000 0

```

```output3
-1

```






```input4
8 3
1 15
5 10
8 1
0 -5 -5 -5 0 -5 -5 0

```

```output4
7
2 1 3
```




## Note

<p>The picture illustrates the first example:</p><center> <img class="tex-graphics" src="./29703/file/C6paWL0L.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
