## ��Ŀ����
����һ������  $a_1,a_2,\cdots,a_n$ ��  $k,p$��

��  $S_{i,j}=\sum\limits_{k=i}^ja_k$����
 $$\mathit{Answer}=\min\{S_{i,j}\bmod p\ |\ S_{i,j}\bmod p\ge k\}$$
���У� $i\le j, \{S_{i,j}\bmod p\ |\ S_{i,j}\bmod p\ge k\}\ne\varnothing$��

## �����ʽ
��һ������������  $n,k,p$��

�ڶ���  $n$ ������������ʾ  $a_1,a_2,\cdots,a_n$��

## �����ʽ
һ��һ������������ʾ  $\mathit{Answer}$��

```input1
7 2 17
12
13
15
11
16
26
11
```

```output1
2
```

## ��ʾ
### ���ݷ�Χ

���� $100\%$ �����ݣ� $1\le n\le10^5$��$1\le k,p,a_i\le10^{18}$��

