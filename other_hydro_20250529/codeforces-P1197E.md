## Description

<div><p>There are famous Russian nesting dolls named matryoshkas sold in one of the souvenir stores nearby, and you'd like to buy several of them. The store has $n$ different matryoshkas. Any matryoshka is a figure of volume $out_i$ with an empty space inside of volume $in_i$ (of course, $out_i &gt; in_i$).</p><p>You don't have much free space inside your bag, but, fortunately, you know that matryoshkas can be nested one inside another. Formally, let's call a set of matryoshkas <span class="tex-font-style-it">nested</span> if we can rearrange dolls in such a way, that the first doll can be nested inside the second one, the second doll ！ inside the third one and so on. Matryoshka $i$ can be nested inside matryoshka $j$ if $out_i \le in_j$. So only the last doll will take space inside your bag.</p><p>Let's call <span class="tex-font-style-it">extra space</span> of a nested set of dolls as a total volume of empty space inside this structure. Obviously, it's equal to $in_{i_1} + (in_{i_2} - out_{i_1}) + (in_{i_3} - out_{i_2}) + \dots + (in_{i_k} - out_{i_{k-1}})$, where $i_1$, $i_2$, ..., $i_k$ are the indices of the chosen dolls in the order they are nested in each other.</p><p>Finally, let's call a nested subset of the given sequence as <span class="tex-font-style-it">big enough</span> if there isn't any doll from the sequence that can be added to the nested subset without breaking its nested property.</p><p>You want to buy many matryoshkas, so you should choose a <span class="tex-font-style-it">big enough</span> nested subset to buy it. But you will be disappointed if too much space in your bag will be wasted, so you want to choose a big enough subset so that its <span class="tex-font-style-it">extra space</span> is minimum possible among all big enough subsets. Now you wonder, how many different nested subsets meet these conditions (they are big enough, and there is no big enough subset such that its extra space is less than the extra space of the chosen subset). Two subsets are considered different if there exists at least one index $i$ such that one of the subsets contains the $i$-th doll, and another subset doesn't.</p><p>Since the answer can be large, print it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the number of matryoshkas.</p><p>The next $n$ lines contain a description of each doll: two integers $out_i$ and $in_i$ ($1 \le in_i &lt; out_i \le 10^9$) ！ the outer and inners volumes of the $i$-th matryoshka.</p></div><div class="output-specification"><p>Print one integer ！ the number of big enough nested subsets such that extra space of each of these subsets is minimum possible. Since the answer can be large, print it modulo $10^9 + 7$.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$) ！ the number of matryoshkas.</p><p>The next $n$ lines contain a description of each doll: two integers $out_i$ and $in_i$ ($1 \le in_i &lt; out_i \le 10^9$) ！ the outer and inners volumes of the $i$-th matryoshka.</p>

## Output

<p>Print one integer ！ the number of big enough nested subsets such that extra space of each of these subsets is minimum possible. Since the answer can be large, print it modulo $10^9 + 7$.</p>

## Samples

```input1
7
4 1
4 2
4 2
2 1
5 4
6 4
3 2
```

```output1
6
```




## Note

<p>There are $6$ big enough nested subsets with minimum possible extra space in the example: </p><ul> <li> $\{1, 5\}$: we can't add any other matryoshka and keep it nested; it's extra space is $1$; </li><li> $\{1, 6\}$; </li><li> $\{2, 4, 5\}$; </li><li> $\{2, 4, 6\}$; </li><li> $\{3, 4, 5\}$; </li><li> $\{3, 4, 6\}$. </li></ul><p>There are no more "good" subsets because, for example, subset $\{6, 7\}$ is not big enough (we can add the $4$-th matryoshka to it) or subset $\{4, 6, 7\}$ has extra space equal to $2$.</p>
