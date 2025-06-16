## ��Ŀ����

In an edge-weighted tree, the xor-length of a path $p$ is defined as the xor sum of the weights of edges on $p$:

$$_{xor}length(p)=\oplus_{e \in p}w(e)$$

$\oplus$ is the xor operator.

We say a path the xor-longest path if it has the largest xor-length. Given an edge-weighted tree with $n$ nodes, can you find the xor-longest path?

����һ�� $n$ ����Ĵ�Ȩ�����������������·����

## �����ʽ

The input contains several test cases. The first line of each test case contains an integer $n$, The following $n-1$ lines each contains three integers $u, v, w$ ($0 \le u \lt n$, $0 \le v \lt n$), which means there is an edge between node $u$ and $v$ of length $w$.

## �����ʽ

For each test case output the xor-length of the xor-longest path.

```input1
4
1 2 3
2 3 4
2 4 6
```
```output1
7
```

## ����˵��

The xor-longest path is $1 \to 2 \to 3$, which has length $7$ ($3 \oplus 4$).

## ��ʾ

ע�⣺����±�� $1$ ��ʼ�� $n$��

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$1 \le n \le 10^5$��$0 \le w \lt 2^{31}$��

