## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"><a href="https://soundcloud.com/decabat/second-dark-matter-battle?in=decabat/sets/best-of-pokemon-super-mystery">Second Dark Matter Battle - Pokemon Super Mystery Dungeon</a></span></div><div class="epigraph-source">⠀</div></div><p>Bessie has recently started playing a famous card game. In the game, there is only one deck of cards, consisting of $a$ "draw $0$" cards, $b$ "draw $1$" cards, $c$ "draw $2$" cards, and $5$ special cards. At the start of the game, all cards are in the randomly shuffled deck.</p><p>Bessie starts the game by drawing the top $5$ cards of the deck. She may then play "draw $x$" cards from the hand to draw the next $x$ cards from the top of the deck. Note that every card can only be played once, special cards cannot be played, and if Bessie uses a "draw $2$" card when there is only $1$ card remaining in the deck, then she simply draws that remaining card. Bessie wins if she draws all $5$ special cards. </p><p>Since Bessie is not very good at math problems, she wants you to find the probability that she wins, given that the deck is shuffled randomly over all $(a + b + c + 5)!$ possible orderings. It can be shown that this answer can always be expressed as a fraction $\frac{p}{q}$ where $p$ and $q$ are coprime integers. Output $p \cdot q^{-1}$ modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case contains three integers $a$, $b$, and $c$ ($0 \le a, b, c \le 2 \cdot 10^5$)&nbsp;– the number of draw $0$ cards, draw $1$ cards, and draw $2$ cards, respectively.</p><p>It is guaranteed that the sum of $a$ over all test cases does not exceed $2 \cdot 10^5$, the sum of $b$ over all test cases does not exceed $2 \cdot 10^5$, and the sum of $c$ over all test cases does not exceed $2 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the probability that Bessie wins, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>Each test case contains three integers $a$, $b$, and $c$ ($0 \le a, b, c \le 2 \cdot 10^5$)&nbsp;– the number of draw $0$ cards, draw $1$ cards, and draw $2$ cards, respectively.</p><p>It is guaranteed that the sum of $a$ over all test cases does not exceed $2 \cdot 10^5$, the sum of $b$ over all test cases does not exceed $2 \cdot 10^5$, and the sum of $c$ over all test cases does not exceed $2 \cdot 10^5$. </p>

## Output

<p>For each test case, output a single integer&nbsp;— the probability that Bessie wins, modulo $998\,244\,353$.</p>





```input1|2,4
4
1 1 1
0 0 0
5 3 7
3366 1434 1234
```




```output1
903173463
1
35118742
398952013
```



## Note

<p>In the first case, we have $1$ of each type of "draw" card and $5$ special cards. There are $30\,720$ starting decks where Bessie will win by drawing the top $5$ cards and $40\,320$ starting decks in total. Thus, the probability of Bessie winning is $\frac{30\,720}{40\,320} = \frac{16}{21}$. </p><p>One example of a winning starting deck is, top to bottom, </p><ol> <li> "Special", </li><li> "Draw $1$", </li><li> "Special", </li><li> "Special", </li><li> "Draw $0$", </li><li> "Draw $2$", </li><li> "Special", </li><li> "Special". </li></ol><p>One example of a losing starting deck is:</p><ol> <li> "Special", </li><li> "Draw $1$", </li><li> "Special", </li><li> "Special", </li><li> "Draw $0$", </li><li> "Special", </li><li> "Special", </li><li> "Draw $2$". </li></ol>
