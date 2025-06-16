## Description

<div><p>You and Nene are playing a card game. The deck with $2n$ cards is used to play this game. Each card has an integer from $1$ to $n$ on it, and each of integers $1$ through $n$ appears exactly on $2$ cards. Additionally, there is a table where cards are placed during the game (initially, the table is empty).</p><p>In the beginning of the game, these $2n$ cards are distributed between you and Nene so that each player receives $n$ cards. </p><p>After it, you and Nene alternatively take $2n$ turns, i.e. each person takes $n$ turns, <span class="tex-font-style-bf">starting with you</span>. On each turn:</p><ul> <li> The player whose turn is it selects one of the cards in his hand. Let $x$ be the number on it. </li><li> The player whose turn is it receives $1$ point if there is already a card with the integer $x$ on the table (otherwise, he receives no points). After it, he places the selected card with the integer $x$ on the table. </li></ul><p>Note that turns are made publicly: each player can see all the cards on the table at each moment.</p><p>Nene is very smart so she always selects cards optimally in order to maximize her score in the end of the game (after $2n$ rounds). If she has several optimal moves, she selects the move that minimizes your score in the end of the game.</p><p>More formally, Nene always takes turns optimally in order to maximize her score in the end of the game in the first place and to minimize your score in the end of the game in the second place.</p><p>Assuming that the cards are already distributed and cards in your hand have integers $a_1, a_2, \ldots, a_n$ written on them, what is the maximum number of points you can get by taking your turns optimally?</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of test cases follows.</p><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of cards you and Nene receive in the beginning of the game.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;！ the integers on the cards in your hand. It is guaranteed that each integer from $1$ through $n$ appears in the sequence $a_1, a_2, \ldots, a_n$ at most $2$ times.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output one integer: the maximum number of points you can get.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of test cases follows.</p><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of cards you and Nene receive in the beginning of the game.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$)&nbsp;！ the integers on the cards in your hand. It is guaranteed that each integer from $1$ through $n$ appears in the sequence $a_1, a_2, \ldots, a_n$ at most $2$ times.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output one integer: the maximum number of points you can get.</p>





```input1|2,3,6,7,10,11
5
4
1 1 2 3
8
7 4 1 2 8 8 5 5
8
7 1 4 5 3 4 2 6
3
1 2 3
1
1
```




```output1
1
2
1
0
0
```



## Note

<p>In the first test case, the integers written on your cards are $1$, $1$, $2$ and $3$. The integers written on Nene's cards are $2$, $3$, $4$ and $4$. The game may proceed as follows:</p><ol> <li> You select one of the cards with an integer $1$ written on it and place it on the table. </li><li> Nene selects one of the cards with an integer $4$ written on it and places it on the table. </li><li> You select the card with an integer $1$ written on it, receive $1$ point, and place the selected card on the table. </li><li> Nene selects the card with an integer $4$ written on it, receive $1$ point, and places the selected card on the table. </li><li> You select the card with an integer $2$ written on it and place it on the table. </li><li> Nene selects the card with an integer $2$ written on it, receive $1$ point, and places the selected card on the table. </li><li> You select the card with an integer $3$ written on it and place it on the table. </li><li> Nene selects the card with an integer $3$ written on it, receive $1$ point, and places the selected card on the table. </li></ol><p>At the end of the game, you scored $1$ point, and Nene scored $3$. It can be shown that you cannot score more than $1$ point if Nene plays optimally, so the answer is $1$.</p><p>In the second test case, if both players play optimally, you score $2$ points and Nene scores $6$ points.</p>
