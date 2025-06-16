## Description

<div><p>Alice and Bob are playing a game. They have $n$ cards numbered from $1$ to $n$. At the beginning of the game, some of these cards are given to Alice, and the rest are given to Bob.</p><p>Card with number $i$ beats card with number $j$ if and only if $i &gt; j$, <span class="tex-font-style-bf">with one exception</span>: card $1$ beats card $n$.</p><p>The game continues as long as each player has at least one card. During each turn, the following occurs:</p><ol> <li> Alice chooses one of her cards and places it face up on the table; </li><li> Bob, seeing Alice's card, chooses one of his cards and places it face up on the table; </li><li> if Alice's card beats Bob's card, both cards are taken by Alice. Otherwise, both cards are taken by Bob. </li></ol><p>A player can use a card that they have taken during one of the previous turns.</p><p>The player who has no cards at the beginning of a turn loses. Determine who will win if both players play optimally.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 5000$) ！ the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains a single integer $n$ ($2 \le n \le 50$) ！ the number of cards; </li><li> the second line contains $n$ characters, each either <span class="tex-font-style-tt">A</span> or <span class="tex-font-style-tt">B</span>. If the $i$-th character is <span class="tex-font-style-tt">A</span>, then card number $i$ is initially given to Alice; otherwise, it is given to Bob. </li></ul><p>Additional constraint on the input: in each test case, at least one card is initially given to Alice, and at least one card is initially given to Bob.</p></div><div class="output-specification"><p>For each test case, output <span class="tex-font-style-tt">Alice</span> if Alice wins with optimal play, or <span class="tex-font-style-tt">Bob</span> if Bob wins. It can be shown that if both players play optimally, the game will definitely end in a finite number of turns with one of the players winning.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 5000$) ！ the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains a single integer $n$ ($2 \le n \le 50$) ！ the number of cards; </li><li> the second line contains $n$ characters, each either <span class="tex-font-style-tt">A</span> or <span class="tex-font-style-tt">B</span>. If the $i$-th character is <span class="tex-font-style-tt">A</span>, then card number $i$ is initially given to Alice; otherwise, it is given to Bob. </li></ul><p>Additional constraint on the input: in each test case, at least one card is initially given to Alice, and at least one card is initially given to Bob.</p>

## Output

<p>For each test case, output <span class="tex-font-style-tt">Alice</span> if Alice wins with optimal play, or <span class="tex-font-style-tt">Bob</span> if Bob wins. It can be shown that if both players play optimally, the game will definitely end in a finite number of turns with one of the players winning.</p>





```input1|2,3,6,7,10,11,14,15
8
2
AB
2
BA
4
ABAB
4
BABA
3
BAA
5
AAAAB
5
BAAAB
6
BBBAAA
```




```output1
Alice
Bob
Bob
Bob
Alice
Alice
Bob
Alice
```



## Note

<p>In the first test case, Alice has only one card, and Bob has only one card. Since Alice's card beats Bob's card, she wins after the first turn.</p><p>In the second test case, Alice has only one card, and Bob has only one card. Since Bob's card beats Alice's card, he wins after the first turn.</p><p>In the third test case, there are two possible game scenarios:</p><ul> <li> if Alice plays the card $1$ on the first turn, Bob can respond with the card $2$ and take both cards. Then, Alice has to play the card $3$ on the second turn, and Bob will respond by playing the card $4$. Then, he wins; </li><li> if Alice plays the card $3$ on the first turn, Bob can respond with the card $4$ and take both cards. Then, Alice has to play the card $1$, and Bob can respond either with the card $2$ or the card $3$. Then, he wins. </li></ul><p>In the fourth test case, there are two possible game scenarios:</p><ul> <li> if Alice plays the card $2$ on the first turn, Bob can respond with the card $3$ and take both cards. Then, Alice has to play the card $4$ on the second turn, and Bob will respond by playing the card $1$. Then, he wins; </li><li> if Alice plays the card $4$ on the first turn, Bob can respond with the card $1$ and take both cards. Then, Alice has to play the card $2$, and Bob can respond either with the card $3$ or the card $4$. Then, he wins. </li></ul>
