## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc212/tasks/abc212_c

���줾�� $ N $ ����$ M $ ��������������ʤ� $ 2 $ �Ĥ����� $ A=(A_1,A_2,\ \ldots\ ,A_N) $ �� $ B=(B_1,\ \ldots\ ,B_M) $ ���뤨���ޤ���

���줾������Ф��� $ 1 $ �Ĥ���Ҫ�ؤ��x����Ȥ��� $ 2 $ �Ĥ΂��β����С�������ʤ���� $ \displaystyle\ \min_{\ 1\leq\ i\leq\ N}\displaystyle\min_{1\leq\ j\leq\ M}\ \lvert\ A_i-B_j\rvert $ �����Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ M $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $ $ B_1 $ $ B_2 $ $ \ldots $ $ B_M $

## �����ʽ
�𤨤�������衣

## ��Ŀ����
�����������ȷֱ�Ϊ $N$ �� $M$ ������������ $A$ �� $B$

��:

$A=(A_1,A_2,...,A_N)N$

$B=(B_1,B_2,...,B_M)M$

�� ��$A$ �� $B$ �ֱ�ȡ��������һ��Ԫ�ص��ܴﵽ����С��ֵ�ľ���ֵΪ���� 

��:
$ \displaystyle\ \min_{\ 1\leq\ i\leq\ N}\displaystyle\min_{1\leq\ j\leq\ M}\ \lvert\ A_i-B_j\rvert $

```input1
2 2
1 6
4 9
```

```output1
2
```

```input2
1 1
10
10
```

```output2
0
```

```input3
6 8
82 76 82 82 71 70
17 39 67 2 45 35 22 24
```

```output3
3
```

## ��ʾ
### �Ƽs

- $ 1\ \leq\ N,M\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 10^9 $
- $ 1\ \leq\ B_i\ \leq\ 10^9 $
- ������ȫ�������Ǥ��롣

### Sample Explanation 1

���줾������Ф��� $ 1 $ �Ĥ���Ҫ�ؤ��x����Ȥ��� $ 2 $ �Ĥ΂��β�Ȥ��Ƥ���ä�Τϡ� $ \lvert\ 1-4\rvert=3 $ �� $ \lvert\ 1-9\rvert=8 $ �� $ \lvert\ 6-4\rvert=2 $ �� $ \lvert\ 6-9\rvert=3 $ �� $ 4 $ �ĤǤ��� �����Ф���С�Ǥ��� $ 2 $ ��������ޤ���

