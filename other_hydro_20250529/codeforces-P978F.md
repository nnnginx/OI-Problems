## Description

<div><p>In BerSoft $n$ programmers work, the programmer $i$ is characterized by a skill $r_i$.</p><p>A programmer $a$ can be a mentor of a programmer $b$ if and only if the skill of the programmer $a$ is strictly greater than the skill of the programmer $b$ $(r_a &gt; r_b)$ and programmers $a$ and $b$ are not in a quarrel.</p><p>You are given the skills of each programmers and a list of $k$ pairs of the programmers, which are in a quarrel (pairs are unordered). For each programmer $i$, find the number of programmers, for which the programmer $i$ can be a mentor.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ $(2 \le n \le 2 \cdot 10^5$, $0 \le k \le \min(2 \cdot 10^5, \frac{n \cdot (n - 1)}{2}))$ �� total number of programmers and number of pairs of programmers which are in a quarrel.</p><p>The second line contains a sequence of integers $r_1, r_2, \dots, r_n$ $(1 \le r_i \le 10^{9})$, where $r_i$ equals to the skill of the $i$-th programmer.</p><p>Each of the following $k$ lines contains two distinct integers $x$, $y$ $(1 \le x, y \le n$, $x \ne y)$ �� pair of programmers in a quarrel. The pairs are unordered, it means that if $x$ is in a quarrel with $y$ then $y$ is in a quarrel with $x$. Guaranteed, that for each pair $(x, y)$ there are no other pairs $(x, y)$ and $(y, x)$ in the input.</p></div><div class="output-specification"><p>Print $n$ integers, the $i$-th number should be equal to the number of programmers, for which the $i$-th programmer can be a mentor. Programmers are numbered in the same order that their skills are given in the input.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ $(2 \le n \le 2 \cdot 10^5$, $0 \le k \le \min(2 \cdot 10^5, \frac{n \cdot (n - 1)}{2}))$ �� total number of programmers and number of pairs of programmers which are in a quarrel.</p><p>The second line contains a sequence of integers $r_1, r_2, \dots, r_n$ $(1 \le r_i \le 10^{9})$, where $r_i$ equals to the skill of the $i$-th programmer.</p><p>Each of the following $k$ lines contains two distinct integers $x$, $y$ $(1 \le x, y \le n$, $x \ne y)$ �� pair of programmers in a quarrel. The pairs are unordered, it means that if $x$ is in a quarrel with $y$ then $y$ is in a quarrel with $x$. Guaranteed, that for each pair $(x, y)$ there are no other pairs $(x, y)$ and $(y, x)$ in the input.</p>

## Output

<p>Print $n$ integers, the $i$-th number should be equal to the number of programmers, for which the $i$-th programmer can be a mentor. Programmers are numbered in the same order that their skills are given in the input.</p>

## Samples

```input1
4 2
10 4 10 15
1 2
4 3

```

```output1
0 0 1 2 

```






```input2
10 4
5 4 1 5 4 3 7 1 2 5
4 6
2 1
10 8
3 5

```

```output2
5 4 0 5 3 3 9 0 2 5 

```




## Note

<p>In the first example, the first programmer can not be mentor of any other (because only the second programmer has a skill, lower than first programmer skill, but they are in a quarrel). The second programmer can not be mentor of any other programmer, because his skill is minimal among others. The third programmer can be a mentor of the second programmer. The fourth programmer can be a mentor of the first and of the second programmers. He can not be a mentor of the third programmer, because they are in a quarrel.</p>
