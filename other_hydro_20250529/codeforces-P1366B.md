## Description

<div><p>You are given an array consisting of $n$ integers $a_1$, $a_2$, ..., $a_n$. Initially $a_x = 1$, all other elements are equal to $0$.</p><p>You have to perform $m$ operations. During the $i$-th operation, you choose two indices $c$ and $d$ such that $l_i \le c, d \le r_i$, and swap $a_c$ and $a_d$.</p><p>Calculate the number of indices $k$ such that it is possible to choose the operations so that $a_k = 1$ in the end.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;�� the number of test cases. Then the description of $t$ testcases follow.</p><p>The first line of each test case contains three integers $n$, $x$ and $m$ ($1 \le n \le 10^9$; $1 \le m \le 100$; $1 \le x \le n$).</p><p>Each of next $m$ lines contains the descriptions of the operations; the $i$-th line contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$).</p></div><div class="output-specification"><p>For each test case print one integer �� the number of indices $k$ such that it is possible to choose the operations so that $a_k = 1$ in the end.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;�� the number of test cases. Then the description of $t$ testcases follow.</p><p>The first line of each test case contains three integers $n$, $x$ and $m$ ($1 \le n \le 10^9$; $1 \le m \le 100$; $1 \le x \le n$).</p><p>Each of next $m$ lines contains the descriptions of the operations; the $i$-th line contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$).</p>

## Output

<p>For each test case print one integer �� the number of indices $k$ such that it is possible to choose the operations so that $a_k = 1$ in the end.</p>

## Samples

```input1
3
6 4 3
1 6
2 3
5 5
4 1 2
2 4
1 2
3 3 2
2 3
1 2
```

```output1
6
2
3
```




## Note

<p>In the first test case, it is possible to achieve $a_k = 1$ for every $k$. To do so, you may use the following operations:</p><ol> <li> swap $a_k$ and $a_4$; </li><li> swap $a_2$ and $a_2$; </li><li> swap $a_5$ and $a_5$. </li></ol><p>In the second test case, only $k = 1$ and $k = 2$ are possible answers. To achieve $a_1 = 1$, you have to swap $a_1$ and $a_1$ during the second operation. To achieve $a_2 = 1$, you have to swap $a_1$ and $a_2$ during the second operation.</p>
