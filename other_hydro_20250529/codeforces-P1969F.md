## Description

<div><p>There is a deck of $n$ cards, each card has one of $k$ types. You are given the sequence $a_1, a_2, \dots, a_n$ denoting the types of cards in the deck from top to bottom. Both $n$ and $k$ are even numbers.</p><p>You play a game with these cards. First, you draw $k$ topmost cards from the deck. Then, the following happens each turn of the game:</p><ul> <li> you choose <span class="tex-font-style-bf">exactly</span> two cards from your hand and play them. If these cards have the same type, you earn a coin; </li><li> then, if the deck is not empty, you draw <span class="tex-font-style-bf">exactly</span> two top cards from it; </li><li> then, if both your hand and your deck are empty, the game ends. Otherwise, the new turn begins. </li></ul><p>You have to calculate the maximum number of coins you can earn during the game.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($2 \le k \le n \le 1000$, both $n$ and $k$ are even).</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le k$).</p></div><div class="output-specification"><p>Print one integer ¡ª the maximum number of coins you can earn.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($2 \le k \le n \le 1000$, both $n$ and $k$ are even).</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le k$).</p>

## Output

<p>Print one integer ¡ª the maximum number of coins you can earn.</p>





```input1|
4 2
1 2 1 2
```




```input2|
8 2
2 1 2 2 1 2 1 2
```




```input3|
4 4
1 2 1 2
```




```input4|
6 4
3 2 3 1 2 1
```




```input5|
6 4
3 2 3 3 2 1
```




```input6|
18 6
5 6 1 1 6 5 4 1 5 1 1 6 2 6 2 2 6 3
```




```input7|
8 4
1 2 3 4 4 3 1 2
```




```input8|
8 4
1 2 3 4 4 3 3 2
```




```output1
0
```




```output2
1
```




```output3
2
```




```output4
3
```




```output5
2
```




```output6
6
```




```output7
2
```




```output8
3
```


