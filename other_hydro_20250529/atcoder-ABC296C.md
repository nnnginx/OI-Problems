## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc296/tasks/abc296_c

�L�� $ N $ ������ $ A=(A_1,\ldots,A_N) $ ���뤨���ޤ���

$ 1\leq\ i,j\ \leq\ N $ �Ǥ���M $ (i,j) $ �Ǥ��äơ�$ A_i-A_j=X $ �Ȥʤ��Τ����ڤ��뤫�ɤ����ж����Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ X $ $ A_1 $ $ \ldots $ $ A_N $

## �����ʽ
$ 1\leq\ i,j\ \leq\ N $ �Ǥ���M $ (i,j) $ �Ǥ��äơ�$ A_i-A_j=X $ �Ȥʤ��Τ����ڤ���Ȥ� `Yes`�����ڤ��ʤ��Ȥ� `No` �ȳ������衣

## ��Ŀ����
��һ������Ϊ $n$ ������ $a$������һ���� $x$��ȷ���Ƿ����һ�� $(i,j)$ ���� $a_i-a_j=x$��

Translated by @[Zealous_YH](https://www.luogu.com.cn/user/399150)

```input1
6 5
3 1 4 1 5 9
```

```output1
Yes
```

```input2
6 -4
-2 -7 -1 -8 -2 -8
```

```output2
No
```

```input3
2 0
141421356 17320508
```

```output3
Yes
```

## ��ʾ
### �Ƽs

- $ 2\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ -10^9\ \leq\ A_i\ \leq\ 10^9 $
- $ -10^9\ \leq\ X\ \leq\ 10^9 $
- ������ȫ�������Ǥ���
 
### Sample Explanation 1

$ A_6-A_3=9-4=5 $ �Ǥ���

### Sample Explanation 2

$ A_i-A_j=-4 $ �Ȥʤ�M $ (i,j) $ �ϴ��ڤ��ޤ���

### Sample Explanation 3

$ A_1-A_1=0 $ �Ǥ���

