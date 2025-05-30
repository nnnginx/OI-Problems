## Description

<div><p>You are given a permutation $a_1, a_2, \dots, a_n$ of numbers from $1$ to $n$. Also, you have $n$ sets $S_1,S_2,\dots, S_n$, where $S_i=\{a_i\}$. Lastly, you have a variable $cnt$, representing the current number of sets. Initially, $cnt = n$.</p><p>We define two kinds of functions on sets:</p><p>$f(S)=\min\limits_{u\in S} u$;</p><p>$g(S)=\max\limits_{u\in S} u$.</p><p>You can obtain a new set by merging two sets $A$ and $B$, if they satisfy $g(A)&lt;f(B)$ (Notice that the old sets do not disappear).</p><p>Formally, you can perform the following sequence of operations:</p><ul><li><p>$cnt\gets cnt+1$;</p></li><li><p>$S_{cnt}=S_u\cup S_v$, you are free to choose $u$ and $v$ for which $1\le u, v &lt; cnt$ and which satisfy $g(S_u)&lt;f(S_v)$.</p></li></ul><p>You are required to obtain some specific sets.</p><p>There are $q$ requirements, each of which contains two integers $l_i$,$r_i$, which means that there must exist a set $S_{k_i}$ ($k_i$ is the ID of the set, you should determine it) which equals $\{a_u\mid l_i\leq u\leq r_i\}$, which is, the set consisting of all $a_i$ with indices between $l_i$ and $r_i$.</p><p>In the end you must ensure that $cnt\leq 2.2\times 10^6$. Note that you <span class="tex-font-style-bf">don't</span> have to minimize $cnt$. It is guaranteed that a solution under given constraints exists.</p></div><div class="input-specification"><p>The first line contains two integers $n,q$ $(1\leq n \leq 2^{12},1 \leq q \leq 2^{16})$ &nbsp;�� the length of the permutation and the number of needed sets correspondently.</p><p>The next line consists of $n$ integers $a_1,a_2,\cdots, a_n$ ($1\leq a_i\leq n$, $a_i$ are pairwise distinct) &nbsp;�� given permutation.</p><p>$i$-th of the next $q$ lines contains two integers $l_i,r_i$ $(1\leq l_i\leq r_i\leq n)$, describing a requirement of the $i$-th set.</p></div><div class="output-specification"><p>It is guaranteed that a solution under given constraints exists.</p><p>The first line should contain one integer $cnt_E$ $(n\leq cnt_E\leq 2.2\times 10^6)$, representing the number of sets after all operations.</p><p>$cnt_E-n$ lines must follow, each line should contain two integers $u$, $v$ ($1\leq u, v\leq cnt'$, where $cnt'$ is the value of $cnt$ before this operation), meaning that you choose $S_u$, $S_v$ and perform a merging operation. In an operation, $g(S_u)&lt;f(S_v)$ must be satisfied.</p><p>The last line should contain $q$ integers $k_1,k_2,\cdots,k_q$ $(1\leq k_i\leq cnt_E)$, representing that set $S_{k_i}$ is the $i$th required set.</p><p><span class="tex-font-style-bf">Please notice the large amount of output.</span></p></div>

## Input

<p>The first line contains two integers $n,q$ $(1\leq n \leq 2^{12},1 \leq q \leq 2^{16})$ &nbsp;�� the length of the permutation and the number of needed sets correspondently.</p><p>The next line consists of $n$ integers $a_1,a_2,\cdots, a_n$ ($1\leq a_i\leq n$, $a_i$ are pairwise distinct) &nbsp;�� given permutation.</p><p>$i$-th of the next $q$ lines contains two integers $l_i,r_i$ $(1\leq l_i\leq r_i\leq n)$, describing a requirement of the $i$-th set.</p>

## Output

<p>It is guaranteed that a solution under given constraints exists.</p><p>The first line should contain one integer $cnt_E$ $(n\leq cnt_E\leq 2.2\times 10^6)$, representing the number of sets after all operations.</p><p>$cnt_E-n$ lines must follow, each line should contain two integers $u$, $v$ ($1\leq u, v\leq cnt'$, where $cnt'$ is the value of $cnt$ before this operation), meaning that you choose $S_u$, $S_v$ and perform a merging operation. In an operation, $g(S_u)&lt;f(S_v)$ must be satisfied.</p><p>The last line should contain $q$ integers $k_1,k_2,\cdots,k_q$ $(1\leq k_i\leq cnt_E)$, representing that set $S_{k_i}$ is the $i$th required set.</p><p><span class="tex-font-style-bf">Please notice the large amount of output.</span></p>

## Samples

```input1
3 2
1 3 2
2 3
1 3
```

```output1
6
3 2
1 3
5 2
4 6
```






```input2
2 4
2 1
1 2
1 2
1 2
1 1
```

```output2
5
2 1
2 1
2 1
5 3 3 1
```




## Note

<p>In the first sample:</p><p>We have $S_1=\{1\},S_2=\{3\},S_3=\{2\}$ initially.</p><p>In the first operation, because $g(S_3)=2&lt;f(S_2)=3$, we can merge $S_3,S_2$ into $S_4=\{2,3\}$.</p><p>In the second operation, because $g(S_1)=1&lt;f(S_3)=2$, we can merge $S_1,S_3$ into $S_5=\{1,2\}$.</p><p>In the third operation, because $g(S_5)=2&lt;f(S_2)=3$, we can merge $S_5,S_2$ into $S_6=\{1,2,3\}$.</p><p>For the first requirement, $S_4=\{2,3\}=\{a_2,a_3\}$, satisfies it, thus $k_1=4$.</p><p>For the second requirement, $S_6=\{1,2,3\}=\{a_1,a_2,a_3\}$, satisfies it, thus $k_2=6$</p><p>Notice that unused sets, identical sets, outputting the same set multiple times, and using sets that are present initially are all allowed.</p>
