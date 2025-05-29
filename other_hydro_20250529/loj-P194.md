## ��Ŀ����

����һ��ģ���⡣

����һ���Ǹ����� $k$ �������� $m$���� Eulerian ��

$$
\left\langle 0\atop k\right\rangle,\left\langle 1\atop k\right\rangle,\dots ,\left\langle {m-1}\atop k\right\rangle
$$

��ģ $p=998244353$ �µĴ𰸡�

���� $\left\langle n\atop k\right\rangle =\sum_{j=0}^k(-1)^j\binom{n+1}{j}(k-j+1)^n$��

## �����ʽ

һ���������� $k,m$��

## �����ʽ

һ�� $m$ �������ֱ�Ϊ $\left\langle 0\atop k\right\rangle \bmod{p},\left\langle 1\atop k\right\rangle \bmod{p},\dots ,\left\langle {m-1}\atop k\right\rangle \bmod{p}$��

```input1
0 10
```

```output1
1 1 1 1 1 1 1 1 1 1
```



$\left\langle n\atop 0\right\rangle =1,\forall n\geq 0$��

```input2
3 10
```

```output2
0 0 0 0 1 26 302 2416 15619 88234
```

## ���ݷ�Χ����ʾ

������� $4$ ��������ÿ�������� $25$ �֣��� $n$ ������������ $0\leq k\leq 10^{n+1},1\leq m\leq 10^{n+1}$��

