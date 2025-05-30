## Description

<div><p>You are given a deck of $n$ cards numbered from $1$ to $n$ (not necessarily in this order in the deck). You have to sort the deck by repeating the following operation. </p><ul> <li> Choose $2 \le k \le n$ and split the deck in $k$ nonempty contiguous parts $D_1, D_2,\dots, D_k$ ($D_1$ contains the first $|D_1|$ cards of the deck, $D_2$ contains the following $|D_2|$ cards and so on). Then reverse the order of the parts, transforming the deck into $D_k, D_{k-1}, \dots, D_2, D_1$ (so, the first $|D_k|$ cards of the new deck are $D_k$, the following $|D_{k-1}|$ cards are $D_{k-1}$ and so on). The internal order of each packet of cards $D_i$ is unchanged by the operation. </li></ul><p>You have to obtain a sorted deck (i.e., a deck where the first card is $1$, the second is $2$ and so on) performing at most $n$ operations. It can be proven that it is always possible to sort the deck performing at most $n$ operations.</p><p><span class="tex-font-style-bf">Examples of operation:</span> The following are three examples of valid operations (on three decks with different sizes). </p><ul> <li> If the deck is <span class="tex-font-style-tt">[3 6 2 1 4 5 7]</span> (so $3$ is the first card and $7$ is the last card), we may apply the operation with $k=4$ and $D_1=$<span class="tex-font-style-tt">[3 6]</span>, $D_2=$<span class="tex-font-style-tt">[2 1 4]</span>, $D_3=$<span class="tex-font-style-tt">[5]</span>, $D_4=$<span class="tex-font-style-tt">[7]</span>. Doing so, the deck becomes <span class="tex-font-style-tt">[7 5 2 1 4 3 6]</span>. </li><li> If the deck is <span class="tex-font-style-tt">[3 1 2]</span>, we may apply the operation with $k=3$ and $D_1=$<span class="tex-font-style-tt">[3]</span>, $D_2=$<span class="tex-font-style-tt">[1]</span>, $D_3=$<span class="tex-font-style-tt">[2]</span>. Doing so, the deck becomes <span class="tex-font-style-tt">[2 1 3]</span>. </li><li> If the deck is <span class="tex-font-style-tt">[5 1 2 4 3 6]</span>, we may apply the operation with $k=2$ and $D_1=$<span class="tex-font-style-tt">[5 1]</span>, $D_2=$<span class="tex-font-style-tt">[2 4 3 6]</span>. Doing so, the deck becomes <span class="tex-font-style-tt">[2 4 3 6 5 1]</span>. </li></ul></div><div class="input-specification"><p>The first line of the input contains one integer $n$ ($1\le n\le 52$) &nbsp;�� the number of cards in the deck.</p><p>The second line contains $n$ integers $c_1, c_2, \dots, c_n$ &nbsp;�� the cards in the deck. The first card is $c_1$, the second is $c_2$ and so on.</p><p>It is guaranteed that for all $i=1,\dots,n$ there is exactly one $j\in\{1,\dots,n\}$ such that $c_j = i$.</p></div><div class="output-specification"><p>On the first line, print the number $q$ of operations you perform (it must hold $0\le q\le n$).</p><p>Then, print $q$ lines, each describing one operation.</p><p>To describe an operation, print on a single line the number $k$ of parts you are going to split the deck in, followed by the size of the $k$ parts: $|D_1|, |D_2|, \dots , |D_k|$. </p><p>It must hold $2\le k\le n$, and $|D_i|\ge 1$ for all $i=1,\dots,k$, and $|D_1|+|D_2|+\cdots + |D_k| = n$.</p><p>It can be proven that it is always possible to sort the deck performing at most $n$ operations. If there are several ways to sort the deck you can output any of them.</p></div>

## Input

<p>The first line of the input contains one integer $n$ ($1\le n\le 52$) &nbsp;�� the number of cards in the deck.</p><p>The second line contains $n$ integers $c_1, c_2, \dots, c_n$ &nbsp;�� the cards in the deck. The first card is $c_1$, the second is $c_2$ and so on.</p><p>It is guaranteed that for all $i=1,\dots,n$ there is exactly one $j\in\{1,\dots,n\}$ such that $c_j = i$.</p>

## Output

<p>On the first line, print the number $q$ of operations you perform (it must hold $0\le q\le n$).</p><p>Then, print $q$ lines, each describing one operation.</p><p>To describe an operation, print on a single line the number $k$ of parts you are going to split the deck in, followed by the size of the $k$ parts: $|D_1|, |D_2|, \dots , |D_k|$. </p><p>It must hold $2\le k\le n$, and $|D_i|\ge 1$ for all $i=1,\dots,k$, and $|D_1|+|D_2|+\cdots + |D_k| = n$.</p><p>It can be proven that it is always possible to sort the deck performing at most $n$ operations. If there are several ways to sort the deck you can output any of them.</p>

## Samples

```input1
4
3 1 2 4
```

```output1
2
3 1 2 1
2 1 3
```






```input2
6
6 5 4 3 2 1
```

```output2
1
6 1 1 1 1 1 1
```






```input3
1
1
```

```output3
0
```




## Note

<p><span class="tex-font-style-bf">Explanation of the first testcase:</span> Initially the deck is <span class="tex-font-style-tt">[3 1 2 4]</span>. </p><ul> <li> The first operation splits the deck as <span class="tex-font-style-tt">[(3) (1 2) (4)]</span> and then transforms it into <span class="tex-font-style-tt">[4 1 2 3]</span>. </li><li> The second operation splits the deck as <span class="tex-font-style-tt">[(4) (1 2 3)]</span> and then transforms it into <span class="tex-font-style-tt">[1 2 3 4]</span>. </li></ul> <span class="tex-font-style-bf">Explanation of the second testcase:</span> Initially the deck is <span class="tex-font-style-tt">[6 5 4 3 2 1]</span>. <ul> <li> The first (and only) operation splits the deck as <span class="tex-font-style-tt">[(6) (5) (4) (3) (2) (1)]</span> and then transforms it into <span class="tex-font-style-tt">[1 2 3 4 5 6]</span>. </li></ul>
