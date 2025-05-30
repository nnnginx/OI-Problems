## Description

<div><p>Nauuo is a girl who loves playing cards.</p><p>One day she was playing cards but found that the cards were mixed with some empty ones.</p><p>There are $n$ cards numbered from $1$ to $n$, and they were mixed with another $n$ empty cards. She piled up the $2n$ cards and drew $n$ of them. The $n$ cards in Nauuo's hands are given. The remaining $n$ cards in the pile are also given in the order from top to bottom.</p><p>In one operation she can choose a card in her hands and play it ！ put it at the bottom of the pile, then draw the top card from the pile.</p><p>Nauuo wants to make the $n$ numbered cards piled up in increasing order (the $i$-th card in the pile from top to bottom is the card $i$) as quickly as possible. Can you tell her the minimum number of operations?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1\le n\le 2\cdot 10^5$) ！ the number of numbered cards.</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($0\le a_i\le n$) ！ the initial cards in Nauuo's hands. $0$ represents an empty card.</p><p>The third line contains $n$ integers $b_1,b_2,\ldots,b_n$ ($0\le b_i\le n$) ！ the initial cards in the pile, given in order from top to bottom. $0$ represents an empty card.</p><p>It is guaranteed that each number from $1$ to $n$ appears exactly once, either in $a_{1..n}$ or $b_{1..n}$.</p></div><div class="output-specification"><p>The output contains a single integer ！ the minimum number of operations to make the $n$ numbered cards piled up in increasing order.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1\le n\le 2\cdot 10^5$) ！ the number of numbered cards.</p><p>The second line contains $n$ integers $a_1,a_2,\ldots,a_n$ ($0\le a_i\le n$) ！ the initial cards in Nauuo's hands. $0$ represents an empty card.</p><p>The third line contains $n$ integers $b_1,b_2,\ldots,b_n$ ($0\le b_i\le n$) ！ the initial cards in the pile, given in order from top to bottom. $0$ represents an empty card.</p><p>It is guaranteed that each number from $1$ to $n$ appears exactly once, either in $a_{1..n}$ or $b_{1..n}$.</p>

## Output

<p>The output contains a single integer ！ the minimum number of operations to make the $n$ numbered cards piled up in increasing order.</p>

## Samples

```input1
3
0 2 0
3 0 1
```

```output1
2
```






```input2
3
0 2 0
1 0 3
```

```output2
4
```






```input3
11
0 0 0 5 0 0 0 4 0 0 11
9 2 6 0 8 1 7 0 3 0 10
```

```output3
18
```




## Note

<p><span class="tex-font-style-bf">Example 1</span></p><p>We can play the card $2$ and draw the card $3$ in the first operation. After that, we have $[0,3,0]$ in hands and the cards in the pile are $[0,1,2]$ from top to bottom.</p><p>Then, we play the card $3$ in the second operation. The cards in the pile are $[1,2,3]$, in which the cards are piled up in increasing order.</p><p><span class="tex-font-style-bf">Example 2</span></p><p>Play an empty card and draw the card $1$, then play $1$, $2$, $3$ in order.</p>
