## Description

<div><p>Sonya decided to organize an exhibition of flowers. Since the girl likes only roses and lilies, she decided that only these two kinds of flowers should be in this exhibition.</p><p>There are $n$ flowers in a row in the exhibition. Sonya can put either a rose or a lily in the $i$-th position. Thus each of $n$ positions should contain exactly one flower: a rose or a lily.</p><p>She knows that exactly $m$ people will visit this exhibition. The $i$-th visitor will visit all flowers from $l_i$ to $r_i$ inclusive. The girl knows that each segment has its own <span class="tex-font-style-it">beauty</span> that is equal to the product of the number of roses and the number of lilies.</p><p>Sonya wants her exhibition to be liked by a lot of people. That is why she wants to put the flowers in such way that the sum of <span class="tex-font-style-it">beauties</span> of all segments would be maximum possible.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1\leq n, m\leq 10^3$)&nbsp;— the number of flowers and visitors respectively.</p><p>Each of the next $m$ lines contains two integers $l_i$ and $r_i$ ($1\leq l_i\leq r_i\leq n$), meaning that $i$-th visitor will visit all flowers from $l_i$ to $r_i$ inclusive.</p></div><div class="output-specification"><p>Print the string of $n$ characters. The $i$-th symbol should be «<span class="tex-font-style-tt">0</span>» if you want to put a rose in the $i$-th position, otherwise «<span class="tex-font-style-tt">1</span>» if you want to put a lily.</p><p>If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1\leq n, m\leq 10^3$)&nbsp;— the number of flowers and visitors respectively.</p><p>Each of the next $m$ lines contains two integers $l_i$ and $r_i$ ($1\leq l_i\leq r_i\leq n$), meaning that $i$-th visitor will visit all flowers from $l_i$ to $r_i$ inclusive.</p>

## Output

<p>Print the string of $n$ characters. The $i$-th symbol should be «<span class="tex-font-style-tt">0</span>» if you want to put a rose in the $i$-th position, otherwise «<span class="tex-font-style-tt">1</span>» if you want to put a lily.</p><p>If there are multiple answers, print any.</p>

## Samples

```input1
5 3
1 3
2 4
2 5

```

```output1
01100
```






```input2
6 3
5 6
1 4
4 6

```

```output2
110010
```




## Note

<p>In the first example, Sonya can put roses in the first, fourth, and fifth positions, and lilies in the second and third positions;</p><ul> <li> in the segment $[1\ldots3]$, there are one rose and two lilies, so the <span class="tex-font-style-it">beauty</span> is equal to $1\cdot 2=2$; </li><li> in the segment $[2\ldots4]$, there are one rose and two lilies, so the <span class="tex-font-style-it">beauty</span> is equal to $1\cdot 2=2$; </li><li> in the segment $[2\ldots5]$, there are two roses and two lilies, so the <span class="tex-font-style-it">beauty</span> is equal to $2\cdot 2=4$. </li></ul><p>The total <span class="tex-font-style-it">beauty</span> is equal to $2+2+4=8$.</p><p>In the second example, Sonya can put roses in the third, fourth, and sixth positions, and lilies in the first, second, and fifth positions;</p><ul> <li> in the segment $[5\ldots6]$, there are one rose and one lily, so the <span class="tex-font-style-it">beauty</span> is equal to $1\cdot 1=1$; </li><li> in the segment $[1\ldots4]$, there are two roses and two lilies, so the <span class="tex-font-style-it">beauty</span> is equal to $2\cdot 2=4$; </li><li> in the segment $[4\ldots6]$, there are two roses and one lily, so the <span class="tex-font-style-it">beauty</span> is equal to $2\cdot 1=2$. </li></ul><p>The total <span class="tex-font-style-it">beauty</span> is equal to $1+4+2=7$.</p>
