## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/agc005/tasks/agc005_b

���̤����Ϥ��������ˤ����L�� $ N $ ����� $ a_1,\ a_2,\ ...,\ a_N $ ���B���ޤ�����

![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_agc005_b/7385c80af4629f5f6d11fed58e1b38d3c006d06d.png)

�����Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ a_1 $ $ a_2 $ $ ... $ $ a_N $

## �����ʽ
$ 1 $ �Ф˴𤨤�������롣

�ʤ���32bit�����ͤ˴𤨤����ޤ�Ȥ��ޤ�ʤ����Ȥ�ע�⤹�뤳�ȡ�

## ��Ŀ����
**Translated by [aoweiyin](https://www.luogu.org/space/show?uid=77834)**

## ���ⷭ��

����һ������Ϊ $N(1\leq N\leq 200,000)$ �ģ��� $(1,2\dots,N)$ �����е����� $a$��

�� $\sum^{N}_ {l=1}\sum^{N}_ {r=l} \min(a_l,a_{l+1},\dots,a_r)$��

#### �����ʽ��

$N$

$a_1\ a_2\dots a_N$




```input1
3
2 1 3
```

```output1
9
```

```input2
4
1 3 2 4
```

```output2
19
```

```input3
8
5 4 8 1 2 6 7 3
```

```output3
85
```

## ��ʾ
### �Ƽs

- $ 1\ �Q\ N\ �Q\ 200,000 $
- $ (a_1,\ a_2,\ ...,\ a_N) $ �� $ (1,\ 2,\ ...,\ N) $ ��K���椨����ΤǤ���

