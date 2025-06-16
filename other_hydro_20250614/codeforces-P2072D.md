## Description

<div><p>Akito got tired of being a simple locksmith at a bank, so he decided to enroll in the Magical Academy and become the best wizard in the world! However, to enroll, he needed to solve a single problem on the exam, which the ambitious hero could not manage.</p><p>In the problem, he was given an array $a$ of length $n$. He needed to minimize the number of inversions$^{\text{∗}}$ in the array after applying the spell <span class="tex-font-style-bf">exactly once</span>. The spell was simple; to apply it, Akito had to choose two numbers $l$ and $r$ such that $1 \le l \le r \le n$ and perform a cyclic shift of the subarray from $l$ to $r$ one position to the left.</p><p>More formally, Akito selects the subarray $[l, r]$ and modifies the array as follows: </p><ul> <li> From the original array $[a_1, a_2, \ldots, a_{l - 1}, \mathbf{ a_l }, \mathbf{ a_{l + 1} } , \mathbf{ \ldots }, \mathbf{ a_{r - 1} }, \mathbf{ a_r }, a_{r + 1}, \ldots, a_{n - 1}, a_n]$, he obtains the array $[a_1, a_2, \ldots, a_{l - 1}, \mathbf{ a_{l + 1} }, \mathbf{ a_{l + 2} }, \mathbf{ \ldots }, \mathbf{ a_{r - 1} }, \mathbf{ a_{r} }, \mathbf{ a_{l} }, a_{r + 1}, \ldots, a_{n - 1}, a_{n}]$. </li></ul><p>Akito is eager to start his studies, but he still hasn't passed the exam. Help him enroll and solve the problem!</p><div class="statement-footnote"><p>$^{\text{∗}}$An inversion in an array $b$ of length $m$ is defined as a pair of indices $(i, j)$ such that $1 \le i &lt; j \le m$ and $b_i &gt; b_j$. For example, in the array $b = [3, 1, 4, 1, 5]$, the inversions are the pairs of indices $(1, 2)$, $(1, 4)$, $(3, 4)$.</p></div></div><div class="input-specification"><p>The first line of input contains a number $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>In the first line of each test case, there is a number $n$ ($1 \le n \le 2000$) — the length of the array $a$.</p><p>In the second line of each test case, there are $n$ numbers $a_i$ ($1 \le a_i \le 2000$) — the elements of the array $a$.</p><p>It is guaranteed that the sum of $n^2$ across all test cases does not exceed $4 \cdot 10^6$.</p></div><div class="output-specification"><p>For each test case, output two numbers $l$ and $r$ ($1 \le l \le r \le n$) — the boundaries of the subarray that should be chosen so that after applying the spell, the number of inversions in the array is minimized.</p><p>If there are multiple suitable pairs of boundaries, you may output any of them.</p></div>

## Input

<p>The first line of input contains a number $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>In the first line of each test case, there is a number $n$ ($1 \le n \le 2000$) — the length of the array $a$.</p><p>In the second line of each test case, there are $n$ numbers $a_i$ ($1 \le a_i \le 2000$) — the elements of the array $a$.</p><p>It is guaranteed that the sum of $n^2$ across all test cases does not exceed $4 \cdot 10^6$.</p>

## Output

<p>For each test case, output two numbers $l$ and $r$ ($1 \le l \le r \le n$) — the boundaries of the subarray that should be chosen so that after applying the spell, the number of inversions in the array is minimized.</p><p>If there are multiple suitable pairs of boundaries, you may output any of them.</p>





```input1|2,3,6,7,10,11,14,15,18,19
9
7
1 4 3 2 5 3 3
6
1 4 3 2 5 3
8
7 6 5 8 4 3 2 1
10
1 1 1 5 1 1 5 6 7 8
2
1337 69
4
2 1 2 1
3
998 244 353
3
1 2 1
9
1 1 2 3 5 8 13 21 34
```




```output1
2 7
2 4
1 8
4 6
1 2
1 4
1 3
2 3
5 5
```



## Note

<p>In the first example, the array $[1, 4, 3, 2, 5, 3, 3]$ will turn into the array $[1, 3, 2, 5, 3, 3, 4]$. The inversions in it are $(2, 3)$, $(4, 5)$, $(4, 6)$ and $(4, 7)$. It can be shown that it is not possible to achieve fewer than $4$ inversions.</p><p>In the second example, the array $[1, 4, 3, 2, 5, 3]$ will turn into $[1, 3, 2, 4, 5, 3]$. The inversions in it are $(2, 3)$, $(4, 6)$, and $(5, 6)$. The pair $l = 2$ and $r = 6$ also works, then the array will turn into $[1, 3, 2, 5, 3, 4]$, which also has $3$ inversions — $(2, 3)$, $(4, 5)$, and $(4, 6)$. It can be shown that it is not possible to achieve fewer than $3$ inversions.</p><p>In the fourth example, choosing $l = 4$ and $r = 6$ transforms the array into $[1, 1, 1, 1, 1, 5, 5, 6, 7, 8]$. It is sorted, and therefore, there are no inversions.</p><p>In the last example, the array is initially sorted, so any operation on a segment of length at least $2$ will only increase the number of inversions.</p>
