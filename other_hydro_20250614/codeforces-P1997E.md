## Description

<div><p>Monocarp is playing a computer game. He starts the game being level $1$. He is about to fight $n$ monsters, in order from $1$ to $n$. The level of the $i$-th monster is $a_i$.</p><p>For each monster in the given order, Monocarp's encounter goes as follows:</p><ul> <li> if Monocarp's level is strictly higher than the monster's level, the monster flees (runs away); </li><li> otherwise, Monocarp fights the monster. </li></ul><p>After every $k$-th fight with a monster (<span class="tex-font-style-bf">fleeing monsters do not count</span>), Monocarp's level increases by $1$. So, his level becomes $2$ after $k$ monsters he fights, $3$ after $2k$ monsters, $4$ after $3k$ monsters, and so on.</p><p>You need to process $q$ queries of the following form:</p><ul> <li> $i~x$: will Monocarp fight the $i$-th monster (or will this monster flee) if the parameter $k$ is equal to $x$? </li></ul></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;！ the number of monsters and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$)&nbsp;！ the levels of the monsters.</p><p>In the $j$-th of the following $q$ lines, two integers $i$ and $x$ ($1 \le i, x \le n$)&nbsp;！ the index of the monster and the number of fights required for a level up in the $j$-th query.</p></div><div class="output-specification"><p>For each query, output "<span class="tex-font-style-tt">YES</span>", if Monocarp will fight the $i$-th monster in this query, and "<span class="tex-font-style-tt">NO</span>", if the $i$-th monster flees.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \le n, q \le 2 \cdot 10^5$)&nbsp;！ the number of monsters and the number of queries.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^5$)&nbsp;！ the levels of the monsters.</p><p>In the $j$-th of the following $q$ lines, two integers $i$ and $x$ ($1 \le i, x \le n$)&nbsp;！ the index of the monster and the number of fights required for a level up in the $j$-th query.</p>

## Output

<p>For each query, output "<span class="tex-font-style-tt">YES</span>", if Monocarp will fight the $i$-th monster in this query, and "<span class="tex-font-style-tt">NO</span>", if the $i$-th monster flees.</p>





```input1|
4 16
2 1 2 1
1 1
2 1
3 1
4 1
1 2
2 2
3 2
4 2
1 3
2 3
3 3
4 3
1 4
2 4
3 4
4 4
```




```input2|
7 15
1 1 2 1 1 1 1
5 3
2 2
2 2
1 6
5 1
5 5
7 7
3 5
7 4
4 3
2 5
1 2
5 6
4 1
6 1
```




```output1
YES
NO
YES
NO
YES
YES
YES
NO
YES
YES
YES
NO
YES
YES
YES
YES
```




```output2
NO
YES
YES
YES
NO
YES
YES
YES
NO
NO
YES
YES
YES
NO
NO
```


