## ��Ŀ����
����һ���������� $A[n\times m]$����һ������ $B[n\times m]$������ $\forall 1\le i\le n,1\le j\le m,B_{i,j}\in[L,R]$����ʹ��ʽֵ��С��

$$\max\begin{cases}\displaystyle\max_{1\le j\le m}\left\{\left|\sum_{i=1}^n\left(A_{i,j}-B_{i,j}\right)\right|\right\}\\\displaystyle\max_{1\le i\le n}\left\{\left|\sum_{j=1}^m\left(A_{i,j}-B_{i,j}\right)\right|\right\}\end{cases}$$

## �����ʽ
��һ���������� $n$��$m$����ʾ����Ĵ�С��

������ $n$ �У�ÿ�� $m$ ���������������� $A$��

���һ������������ $L$��$R$��

## �����ʽ
���һ��һ����������𰸡�

```input1
2 2
0 1
2 1
0 1
```

```output1
1
```

## ��ʾ
���� $100\%$ ���������� $n,m\le200$��$0\le L\le R\le1000$��$0\le A_{i,j}\le1000$��

