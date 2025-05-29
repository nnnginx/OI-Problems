## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">This is the way it always was.</span></div></div> <div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">This is the way it always will be.</span></div></div> <div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it">All will be forgotten again soon...</span></div></div><p>Jellyfish is playing a one-player card game called "Slay the Spire". There are $n$ cards in total numbered from $1$ to $n$. The $i$-th card has <span class="tex-font-style-it">power</span> $c_i$.</p><p>There is a binary string $s$ of length $n$. If $s_i = \texttt{0}$, the $i$-th card is initially in the draw pile. If $s_i = \texttt{1}$, the $i$-th card is initially in Jellyfish's hand.</p><p>Jellyfish will repeat the following process until either her hand or the draw pile is empty. </p><ol> <li> Let $x$ be the power of the card with the largest power in her hand. </li><li> Place a single card with power $x$ back into the draw pile. </li><li> Randomly draw $x$ cards from the draw pile. All subsets of $x$ cards from the draw pile have an equal chance of being drawn. If there are fewer than $x$ cards in the draw pile, Jellyfish will draw all cards. </li></ol><p>At the end of this process, find the probability that Jellyfish can empty the draw pile, modulo $1\,000\,000\,007$.</p><p>Formally, let $M=1\,000\,000\,007$. It can be shown that the answer can be expressed as an irreducible fraction $\frac{p}{q}$, where $p$ and $q$ are integers and $q \not \equiv 0 \pmod{M}$. Output the integer equal to $p \cdot q^{-1} \bmod M$. In other words, output such an integer $x$ that $0 \le x &lt; M$ and $x \cdot q \equiv p \pmod{M}$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\leq t\leq 100$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 120$)&nbsp;！ the number of cards.</p><p>The second line of each test case contains $n$ integers $c_1,c_2,\ldots,c_n$ ($0 \leq c_i \leq n$)&nbsp;！ the powers of the cards. It is guaranteed that $c_1 \leq c_2 \leq \ldots \leq c_n$.</p><p>The third line of each test case contains a binary string $s$ of length $n$. If $s_i = \texttt{0}$, the $i$-th card is initially in the draw pile. If $s_i = \texttt{1}$, the $i$-th card is initially in Jellyfish's hand.</p><p>It is guaranteed that the sum of $n^2$ over all test cases does not exceed $120^2$.</p></div><div class="output-specification"><p>For each test case, output the probability that Jellyfish can empty the draw pile modulo $1\,000\,000\,007$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1\leq t\leq 100$). The description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \leq n \leq 120$)&nbsp;！ the number of cards.</p><p>The second line of each test case contains $n$ integers $c_1,c_2,\ldots,c_n$ ($0 \leq c_i \leq n$)&nbsp;！ the powers of the cards. It is guaranteed that $c_1 \leq c_2 \leq \ldots \leq c_n$.</p><p>The third line of each test case contains a binary string $s$ of length $n$. If $s_i = \texttt{0}$, the $i$-th card is initially in the draw pile. If $s_i = \texttt{1}$, the $i$-th card is initially in Jellyfish's hand.</p><p>It is guaranteed that the sum of $n^2$ over all test cases does not exceed $120^2$.</p>

## Output

<p>For each test case, output the probability that Jellyfish can empty the draw pile modulo $1\,000\,000\,007$.</p>





```input1|2,3,4,8,9,10
4
5
0 1 1 1 2
00100
3
2 3 3
000
10
0 0 0 0 0 0 0 1 1 1
1111011111
20
0 0 0 0 0 0 0 0 0 0 0 0 0 0 1 1 2 3 3 4
00000000001000101010
```




```output1
500000004
0
0
675898154
```



## Note

<p>In the first test case, Jellyfish will keep playing cards with power $1$ until Jellyfish draws a card with power $0$ or power $2$. If Jellyfish draws a card with power $0$, she will eventually empty her hand. If Jellyfish draws a card with power $2$, she will eventually empty the draw pile. Since there is an equal chance of drawing $0$ or $2$, the answer is $\frac{1}{2}$, and $2 \cdot 500\,000\,004 \equiv 1 \pmod {10^9+7}$</p>
