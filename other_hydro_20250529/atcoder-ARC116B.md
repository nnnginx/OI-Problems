## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/arc116/tasks/arc116_b

�L�� $ N $ �������� $ A $ ���뤨���ޤ���$ A $ �οդǤʤ������� $ B $ �� $ 2^N\ -\ 1 $ ������ޤ��������ˤĤ��� $ \max\left(B\right)\ \times\ \min\left(B\right) $ �΂���Ӌ�㤷�����ξt�ͤ�𤨤Ƥ���������

���������𤨤Ϸǳ��˴󤭤��ʤ���Ϥ�����Τǡ� $ 998244353 $ �Ǹ�ä�����𤨤Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## �����ʽ
�𤨤�������衣

## ��Ŀ����
����һ����Ϊ $n$ ������ $A$���� $A$ ������ $2^n-1$ ���ǿ������� $B$ �У������е� $\max\{B\}\times\min\{B\}$ �ĺ͡�

```input1
3
2 4 3
```

```output1
63
```

```input2
1
10
```

```output2
100
```

```input3
7
853983 14095 543053 143209 4324 524361 45154
```

```output3
206521341
```

## ��ʾ
### �Ƽs

- ������ȫ������
- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 0\ \leq\ A_i\ \leq\ 998244352 $

### Sample Explanation 1

$ B $ �Ȥ��ơ����¤� $ 7 $ �Ĥ��������ޤ��� - $ B\ =\ \left(2\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 4 $ - $ B\ =\ \left(4\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 16 $ - $ B\ =\ \left(3\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 9 $ - $ B\ =\ \left(2,\ 4\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 8 $ - $ B\ =\ \left(2,\ 3\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 6 $ - $ B\ =\ \left(4,\ 3\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 12 $ - $ B\ =\ \left(2,\ 4,\ 3\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 8 $ ���Ϥ� $ 7 $ �Ĥ΂����㤷���� $ 63 $ ���𤨤Ǥ���

