## Description

<div><p>When they are bored, Federico and Giada often play the following card game with a deck containing $6n$ cards.</p><p>Each card contains one number between $1$ and $6n$ and each number appears on exactly one card. Initially the deck is sorted, so the first card contains the number $1$, the second card contains the number $2$, $\dots$, and the last one contains the number $6n$.</p><p>Federico and Giada take turns, alternating; Federico starts.</p><p>In his turn, the player takes $3$ contiguous cards from the deck and puts them in his pocket. The order of the cards remaining in the deck is not changed. They play until the deck is empty (after exactly $2n$ turns). At the end of the game both Federico and Giada have $3n$ cards in their pockets.</p><p>You are given the cards in Federico's pocket at the end of the game. Describe a sequence of moves that produces that set of cards in Federico's pocket.</p></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1\le n \le 200$).</p><p>The second line of the input contains $3n$ numbers $x_1, x_2,\ldots, x_{3n}$ ($1 \le x_1 &lt; x_2 &lt;\ldots &lt; x_{3n} \le 6n$) �C the cards in Federico's pocket at the end of the game. </p><p>It is guaranteed that for each test there is at least one sequence of moves that produces such set of cards in Federico's pocket.</p></div><div class="output-specification"><p>Print $2n$ lines, each containing $3$ integers.</p><p>The $i$-th line should contain, in increasing order, the integers $a_i&lt;b_i&lt;c_i$ written on the three cards taken by the player during the $i$-th turn (so taken by Federico if $i$ is odd and by Giada if $i$ is even).</p><p>If there is more than one possible sequence of moves, you can print any.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1\le n \le 200$).</p><p>The second line of the input contains $3n$ numbers $x_1, x_2,\ldots, x_{3n}$ ($1 \le x_1 &lt; x_2 &lt;\ldots &lt; x_{3n} \le 6n$) �C the cards in Federico's pocket at the end of the game. </p><p>It is guaranteed that for each test there is at least one sequence of moves that produces such set of cards in Federico's pocket.</p>

## Output

<p>Print $2n$ lines, each containing $3$ integers.</p><p>The $i$-th line should contain, in increasing order, the integers $a_i&lt;b_i&lt;c_i$ written on the three cards taken by the player during the $i$-th turn (so taken by Federico if $i$ is odd and by Giada if $i$ is even).</p><p>If there is more than one possible sequence of moves, you can print any.</p>

## Samples

```input1
2
2 3 4 9 10 11
```

```output1
9 10 11
6 7 8
2 3 4
1 5 12
```






```input2
5
1 2 3 4 5 9 11 12 13 18 19 20 21 22 23
```

```output2
19 20 21
24 25 26
11 12 13
27 28 29
1 2 3
14 15 16
18 22 23
6 7 8
4 5 9
10 17 30
```




## Note

<p><span class="tex-font-style-bf">Explanation of the first testcase:</span> Initially the deck has $12 = 2\cdot 6$ sorted cards, so the deck is $[1\ 2\ 3\ 4\ 5\ 6\ 7\ 8\ 9\ 10\ 11\ 12]$. </p><ul> <li> During turn $1$, Federico takes the three cards $[9\ 10\ 11]$. After his move, the deck is $[1\ 2\ 3\ 4\ 5\ 6\ 7\ 8\ 12]$. </li><li> During turn $2$, Giada takes the three cards $[6\ 7\ 8]$. After her move, the deck is $[1\ 2\ 3\ 4\ 5\ 12]$. </li><li> During turn $3$, Federico takes the three cards $[2\ 3\ 4]$. After his move, the deck is $[1\ 5\ 12]$. </li><li> During turn $4$, Giada takes the three cards $[1\ 5\ 12]$. After her move, the deck is empty. </li></ul> At the end of the game, the cards in Federico's pocket are $[2\ 3\ 4\ 9\ 10\ 11]$ and the cards in Giada's pocket are $[1\ 5\ 6\ 7\ 8\ 12]$.
