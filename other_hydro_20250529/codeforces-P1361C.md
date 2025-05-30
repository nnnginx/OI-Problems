## Description

<div><p>Johnny's younger sister Megan had a birthday recently. Her brother has bought her a box signed as "<span class="tex-font-style-it">Your beautiful necklace&nbsp;！ do it yourself!</span>". It contains many necklace parts and some magic glue. </p><p>The necklace part is a chain connecting two pearls. Color of each pearl can be defined by a non-negative integer. The magic glue allows Megan to merge two pearls (possibly from the same necklace part) into one. The beauty of a connection of pearls in colors $u$ and $v$ is defined as follows: let $2^k$ be the greatest power of two dividing $u \oplus v$&nbsp;！ <a href="https://en.wikipedia.org/wiki/Exclusive_or#Computer_science">exclusive or</a> of $u$ and $v$. Then the beauty equals $k$. If $u = v$, you may assume that beauty is equal to $20$.</p><p>Each pearl can be combined with another at most once. Merging two parts of a necklace connects them. Using the glue multiple times, Megan can finally build the necklace, which is a cycle made from connected necklace parts (so every pearl in the necklace is combined with precisely one other pearl in it). The beauty of such a necklace is the minimum beauty of a single connection in it. The girl wants to use all available necklace parts to build <span class="tex-font-style-bf">exactly one</span> necklace consisting of <span class="tex-font-style-bf">all of them</span> with the largest possible beauty. Help her!</p></div><div class="input-specification"><p>The first line contains $n$ $(1 \leq n \leq 5 \cdot 10^5)$&nbsp;！ the number of necklace parts in the box. Each of the next $n$ lines contains two integers $a$ and $b$ $(0 \leq a, b &lt; 2^{20})$, which denote colors of pearls presented in the necklace parts. Pearls in the $i$-th line have indices $2i - 1$ and $2i$ respectively.</p></div><div class="output-specification"><p>The first line should contain a single integer $b$ denoting the maximum possible beauty of a necklace built from all given parts.</p><p>The following line should contain $2n$ distinct integers $p_i$ $(1 \leq p_i \leq 2n)$&nbsp;！ the indices of initial pearls in the order in which they appear on a cycle. Indices of pearls belonging to the same necklace part have to appear at neighboring positions in this permutation (so $1\,4\,3\,2$ is not a valid output, whereas $2\,1\,4\,3$ and $4\,3\,1\,2$ are). If there are many possible answers, you can print any.</p></div>

## Input

<p>The first line contains $n$ $(1 \leq n \leq 5 \cdot 10^5)$&nbsp;！ the number of necklace parts in the box. Each of the next $n$ lines contains two integers $a$ and $b$ $(0 \leq a, b &lt; 2^{20})$, which denote colors of pearls presented in the necklace parts. Pearls in the $i$-th line have indices $2i - 1$ and $2i$ respectively.</p>

## Output

<p>The first line should contain a single integer $b$ denoting the maximum possible beauty of a necklace built from all given parts.</p><p>The following line should contain $2n$ distinct integers $p_i$ $(1 \leq p_i \leq 2n)$&nbsp;！ the indices of initial pearls in the order in which they appear on a cycle. Indices of pearls belonging to the same necklace part have to appear at neighboring positions in this permutation (so $1\,4\,3\,2$ is not a valid output, whereas $2\,1\,4\,3$ and $4\,3\,1\,2$ are). If there are many possible answers, you can print any.</p>

## Samples

```input1
5
13 11
11 1
3 5
17 1
9 27
```

```output1
3
8 7 9 10 5 6 1 2 3 4
```






```input2
5
13 11
11 1
3 5
17 1
7 29
```

```output2
2
8 7 10 9 5 6 4 3 2 1
```






```input3
1
1 1
```

```output3
20
2 1
```




## Note

<p>In the first example the following pairs of pearls are combined: $(7, 9)$, $(10, 5)$, $(6, 1)$, $(2, 3)$ and $(4, 8)$. The beauties of connections equal correspondingly: $3$, $3$, $3$, $20$, $20$.</p><p>The following drawing shows this construction.</p><center> <img class="tex-graphics" src="./31196/file/KTiZBBcw.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
