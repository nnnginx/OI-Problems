## Description

<div><p>Monocarp has $n$ pizzas, the $i$-th pizza consists of $a_i$ slices. Pizzas are denoted by uppercase Latin letters from <span class="tex-font-style-tt">A</span> to the $n$-th letter of the Latin alphabet.</p><p>Monocarp also has $m$ friends, and he wants to invite <span class="tex-font-style-bf">exactly two</span> of them to eat pizza. For each friend, Monocarp knows which pizzas that friend likes.</p><p>After the friends arrive at Monocarp's house, for each pizza, the following happens:</p><ul> <li> if the pizza is not liked by any of the two invited friends, Monocarp eats it; </li><li> if the pizza is liked by exactly one of the two invited friends, that friend eats it; </li><li> and if the pizza is liked by both friends, they try to split it. If it consists of an even number of slices, they both eat exactly half of the slices. But if the pizza consists of an odd number of slices, they start quarrelling, trying to decide who will eat an extra slice ！ and Monocarp doesn't like that. </li></ul><p>For each $k$ from $0$ to $\sum a_i$, calculate the number of ways to choose <span class="tex-font-style-bf">exactly two friends</span> to invite so that the friends don't quarrel, and Monocarp eats exactly $k$ slices.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 20$; $2 \le m \le 5 \cdot 10^5$) ！ the number of pizzas and the number of friends, respectively.</p><p>The second line contains $m$ strings $s_1, s_2, \dots, s_m$ ($1 \le |s_i| \le n$), where $s_i$ is a string consisting of <span class="tex-font-style-bf">distinct</span> characters from <span class="tex-font-style-tt">A</span> to the $n$-th letter of the Latin alphabet, denoting which pizzas the $i$-th friend likes. In every string $s_i$, the characters are sorted in lexicographical (alphabetic) order.</p><p>The third line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^4$) ！ the sizes of the pizzas.</p></div><div class="output-specification"><p>Print $\sum a_i + 1$ integers, where the $k$-th integer (starting from $0$) should be the number of ways to choose <span class="tex-font-style-bf">exactly two friends</span> to invite so that the friends don't quarrel, and Monocarp eats exactly $k$ slices.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 20$; $2 \le m \le 5 \cdot 10^5$) ！ the number of pizzas and the number of friends, respectively.</p><p>The second line contains $m$ strings $s_1, s_2, \dots, s_m$ ($1 \le |s_i| \le n$), where $s_i$ is a string consisting of <span class="tex-font-style-bf">distinct</span> characters from <span class="tex-font-style-tt">A</span> to the $n$-th letter of the Latin alphabet, denoting which pizzas the $i$-th friend likes. In every string $s_i$, the characters are sorted in lexicographical (alphabetic) order.</p><p>The third line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2 \cdot 10^4$) ！ the sizes of the pizzas.</p>

## Output

<p>Print $\sum a_i + 1$ integers, where the $k$-th integer (starting from $0$) should be the number of ways to choose <span class="tex-font-style-bf">exactly two friends</span> to invite so that the friends don't quarrel, and Monocarp eats exactly $k$ slices.</p>





```input1|
3 6
A AB ABC AB BC C
2 3 5
```




```output1
4 0 0 1 0 2 0 0 0 0 0
```



## Note

<p>Let's consider all pairs of friends from the first example:</p><ul> <li> if Monocarp invites friends $1$ and $2$, they will eat pizzas $1$ and $2$, and he'll eat the $3$-rd pizza; </li><li> if Monocarp invites friends $1$ and $3$, they will eat all of the pizzas; </li><li> if Monocarp invites friends $1$ and $4$, they will eat pizzas $1$ and $2$, and he'll eat the $3$-rd pizza; </li><li> if Monocarp invites friends $1$ and $5$, they will eat all of the pizzas; </li><li> if Monocarp invites friends $1$ and $6$, they will eat pizzas $1$ and $3$, and he'll eat the $2$-nd pizza; </li><li> if Monocarp invites friends $2$ and $3$, they will quarrel because of the $2$-nd pizza; </li><li> if Monocarp invites friends $2$ and $4$, they will quarrel because of the $2$-nd pizza; </li><li> if Monocarp invites friends $2$ and $5$, they will quarrel because of the $2$-nd pizza; </li><li> if Monocarp invites friends $2$ and $6$, they will eat all of the pizzas; </li><li> if Monocarp invites friends $3$ and $4$, they will quarrel because of the $2$-nd pizza; </li><li> if Monocarp invites friends $3$ and $5$, they will quarrel because of the $2$-nd pizza; </li><li> if Monocarp invites friends $3$ and $6$, they will quarrel because of the $3$-rd pizza; </li><li> if Monocarp invites friends $4$ and $5$, they will quarrel because of the $2$-nd pizza; </li><li> if Monocarp invites friends $4$ and $6$, they will eat all of the pizzas; </li><li> if Monocarp invites friends $5$ and $6$, they will quarrel because of the $3$-rd pizza. </li></ul>
