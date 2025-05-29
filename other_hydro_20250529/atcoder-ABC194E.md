## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc194/tasks/abc194_e

$ \mathrm{mex}(x_1,\ x_2,\ x_3,\ \dots,\ x_k) $ ��$ x_1,\ x_2,\ x_3,\ \dots,\ x_k $ �˺��ޤ�ʤ���С�η�ؓ�����ȶ��x���ޤ���  
 �L�� $ N $ �������� $ A\ =\ (A_1,\ A_2,\ A_3,\ \dots,\ A_N) $ ���뤨���ޤ���  
 $ 0\ \le\ i\ \le\ N\ -\ M $ �򜺤���ȫ�Ƥ����� $ i $ �ˤĤ��� $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2},\ A_{i\ +\ 3},\ \dots,\ A_{i\ +\ M}) $ ��Ӌ�㤷���Ȥ������� $ N\ -\ M\ +\ 1 $ ���΂��Τ�������С�������Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ M $ $ A_1 $ $ A_2 $ $ A_3 $ $ \cdots $ $ A_N $

## �����ʽ
�𤨤�������衣

## ��Ŀ����
- ����һ������Ϊ $N$ ������ $A$���� $A$ �����г���Ϊ $M$ �������������У���С�� $\operatorname{mex}$ ֵ������ $\operatorname{mex}$ Ϊ��������Сδ���ֵ���Ȼ������
- $1\le M\le N\le 15\times 10^5,\ 0\le A_i< N$��

@[hellolin](/user/751017) ��

```input1
3 2
0 0 1
```

```output1
1
```

```input2
3 2
1 1 1
```

```output2
0
```

```input3
3 2
0 1 0
```

```output3
2
```

```input4
7 3
0 0 1 2 0 1 0
```

```output4
2
```

## ��ʾ
### �Ƽs

- $ 1\ \le\ M\ \le\ N\ \le\ 1.5\ \times\ 10^6 $
- $ 0\ \le\ A_i\ \lt\ N $
- �����˺��ޤ�낎��ȫ������

### Sample Explanation 1

\- $ i\ =\ 0 $ �ΤȤ� : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(0,\ 0)\ =\ 1 $ - $ i\ =\ 1 $ �ΤȤ� : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(0,\ 1)\ =\ 2 $ ��ä� $ 1 $ �� $ 2 $ �Τ�������С���Ǥ��� $ 1 $ ���𤨤Ǥ���

### Sample Explanation 2

\- $ i\ =\ 0 $ �ΤȤ� : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(1,\ 1)\ =\ 0 $ - $ i\ =\ 1 $ �ΤȤ� : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(1,\ 1)\ =\ 0 $ �Ȥʤ�ޤ���

### Sample Explanation 3

\- $ i\ =\ 0 $ �ΤȤ� : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(0,\ 1)\ =\ 2 $ - $ i\ =\ 1 $ �ΤȤ� : $ \mathrm{mex}(A_{i\ +\ 1},\ A_{i\ +\ 2})\ =\ \mathrm{mex}(1,\ 0)\ =\ 2 $ �Ȥʤ�ޤ���

