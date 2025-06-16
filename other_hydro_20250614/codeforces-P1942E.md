## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"><a href="https://soundcloud.com/p92402/kaguyas-theme-lunatic-princess">Lunatic Princess - Touhou</a></span></div><div class="epigraph-source">⠀</div></div><p>Farmer Nhoj has brought his cows over to Farmer John's farm to play a game! FJ's farm can be modeled by a number line with walls at points $0$ and $l + 1$. On the farm, there are $2n$ cows, with $n$ of the cows belonging to FJ and the other $n$ belonging to FN. They place each of their cows at a distinct point, and no two FJ's cows nor FN's cows are adjacent. Two cows are adjacent if there are no other cows between them. </p><p>Formally, if $a_1, a_2, \ldots, a_n$ represents the positions of FJ's cows and $b_1, b_2, \ldots, b_n$ represents the positions of FN's cows, then either $0 &lt; a_1 &lt; b_1 &lt; a_2 &lt; b_2 &lt; \ldots &lt; a_n &lt; b_n &lt; l + 1$ or $0 &lt; b_1 &lt; a_1 &lt; b_2 &lt; a_2 &lt; \ldots &lt; b_n &lt; a_n &lt; l + 1$.</p><p>In one move, a farmer chooses a number $k$ $(1 \leq k \leq n)$ and a direction (left or right). Then, that farmer chooses $k$ of his cows and moves them one position towards the chosen direction. A farmer cannot move any of his cows onto the walls or onto another farmer's cow. If a farmer cannot move any cows, then that farmer loses. FJ starts the game, making the first turn.</p><p>Given $l$ and $n$, find the number of possible game configurations for Farmer John to win if both farmers play optimally. It may be the case that the game will continue indefinitely, in which no farmer wins. A configuration is different from another if there is any $i$ such that $a_i$ or $b_i$ is different. Output the answer modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>Each test case contains two integers $l$ and $n$ ($2 \leq l \leq 10^6, 1 \leq n \leq \lfloor \frac{l}{2} \rfloor$)&nbsp;— the length of the number line and the number of cows each farmer will place.</p><p>It is guaranteed the sum of $l$ over all test cases does not exceed $10^6$.</p></div><div class="output-specification"><p>For each test case output an integer: the number of game configurations where Farmer John wins if both farmers play optimally, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains $t$ ($1 \leq t \leq 10^4$)&nbsp;— the number of test cases.</p><p>Each test case contains two integers $l$ and $n$ ($2 \leq l \leq 10^6, 1 \leq n \leq \lfloor \frac{l}{2} \rfloor$)&nbsp;— the length of the number line and the number of cows each farmer will place.</p><p>It is guaranteed the sum of $l$ over all test cases does not exceed $10^6$.</p>

## Output

<p>For each test case output an integer: the number of game configurations where Farmer John wins if both farmers play optimally, modulo $998\,244\,353$.</p>





```input1|2,4
3
2 1
3 1
420 69
```




```output1
0
2
870279412
```



## Note

<p>Let <span class="tex-font-style-tt">J</span> denote FJ's cow, <span class="tex-font-style-tt">N</span> denote FN's cow, and <span class="tex-font-style-tt">_</span> denote an empty space.</p><p>For the first test case, the two possible configurations are <span class="tex-font-style-tt">JN</span> or <span class="tex-font-style-tt">NJ</span>. In both cases, since FJ makes the first turn and cannot make any moves, he cannot win.</p><p>For the second case there are two possible configurations for FJ to win: <span class="tex-font-style-tt">N_J</span> and <span class="tex-font-style-tt">J_N</span>.</p>
