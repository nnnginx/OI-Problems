## ��Ŀ����
DreamGrid has a paper strip with $n$ grids in a line and he has drawn some beautiful patterns in some grids. Unfortunately, his naughty roommate BaoBao drew some other patterns in some other grids when he wasn't at home. Now DreamGrid has to erase BaoBao's patterns without destroying his own patterns.

Let's number the grids from 1 to $n$ from left to right. Each grid either contains DreamGrid's pattern, or contains BaoBao's pattern, or is empty.

Each time, DreamGrid can select two integers $l$ and $r$ (these two integers can be different each time) such that

- $1 \le l \le r \le n$, and
- for all $l \le i \le r$, the $i$-th grid either contains BaoBao's pattern, or is empty,

and change the $i$-th grid to an empty grid for all $l \le i \le r$.

How many ways can DreamGrid change all the grids containing BaoBao's pattern to empty grids by performing the above operation exactly $m$ times? As the answer may be large, please print the answer modulo $10^9 + 7$.

Let $\{(a_1, b_1), (a_2, b_2), \dots (a_m, b_m)\}$ be a valid erasing sequence ($1 \le a_i \le b_i \le n$), where $(a_i, b_i)$ indicates that DreamGrid selects integers $a_i$ and $b_i$ in the $i$-th operation. Let $\{(c_1, d_1), (c_2, d_2), \dots, (c_m, d_m)\}$ be another valid erasing sequence ($1 \le c_i \le d_i \le n$), where $(c_i, d_i)$ indicates that DreamGrid selects integers $c_i$ and $d_i$ in the $i$-th operation. These two sequences are considered different, if there exists an integer $k$ ($1 \le k \le m$) such that $a_k \ne c_k$ or $b_k \ne d_k$.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ ($1 \le T \le 1000$), indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $m$ ($1 \le n \le 100$, $1 \le m \le 10^9$), indicating the number of grids and the number of times to perform the operation.

The second line contains $n$ integers $a_i$ ($a_i \in \{0, 1, 2\}$).

- If $a_i = 0$, the $i$-th grid is empty.
- If $a_i = 1$, the $i$-th grid contains DreamGrid's pattern.
- If $a_i = 2$, the $i$-th grid contains BaoBao's pattern.

It's guaranteed that at most 50 test cases have $n > 50$.

## �����ʽ
For each test case, output one line containing the number of ways modulo $10^9 + 7$.

## ��Ŀ����
�������� $T(1\le T\le100)$. ����ÿ������ :

�������� $n, m(n\le 100, m\le10^9)$. ����������һ������Ϊ $n$ ������ $a$, ��֤ $a_i\in \{0, 1, 2\}$.

����Ҫִ������Ĳ���ǡ�� $m$ �Σ�

- ָ�������� $l, r \le n$, ���� $\forall i\in \mathbf{N}$ �� $i\in[l, r]$, �� $a_i \ne 1$.
- ���������� $i \in [l, r]$ �� $a_i$ ��ֵΪ $0$.

���ж����ֲ�ͬ�Ĳ�����ʽ, ʹ�ý������� $m$ �β�����, $\forall i\in[l, r], a_i \ne 2$. ���ڴ𰸿��ܴܺ�������𰸶� $10^9 + 7$ ȡģ��ֵ.

**ע�� : ����ÿ�����ݵ�, ������ 50 ���������� $n>50$.**

Translated by @[Ja50nY0un9](/user/363302).

```input1
3
2 2
2 0
3 2
2 1 0
3 1
2 1 0
```

```output1
8
3
1
```

