## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/arc111/tasks/arc111_a

������ $ N,\ M $ ���뤨���ޤ���$ \lfloor\ \frac{10^N}{M}\ \rfloor $ �� $ M $ �Ǹ�ä��������Ƥ���������

  $ \lfloor\ x\ \rfloor $ �ˤĤ��� $ \lfloor\ x\ \rfloor $ �ϡ� $ x $ �򳬤��ʤ�������������ޤ������Ȥ��ƤϴΤΤ褦�ˤʤ�ޤ��� - $ \lfloor\ 2.5\ \rfloor\ =\ 2 $
- $ \lfloor\ 3\ \rfloor\ =\ 3 $
- $ \lfloor\ 9.9999999\ \rfloor\ =\ 9 $
- $ \lfloor\ \frac{100}{3}\ \rfloor\ =\ \lfloor\ 33.33...\ \rfloor\ =\ 33 $

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ M $

## �����ʽ
�𤨤�������衣

## ��Ŀ����
���������� $n$ �� $m$��

��� $\left\lfloor\frac{10^n}{m}\right\rfloor \bmod m$ ��ֵ��

$n \le 10^{18},m \le 10^4$��

```input1
1 2
```

```output1
1
```

```input2
2 7
```

```output2
0
```

```input3
1000000000000000000 9997
```

```output3
9015
```

## ��ʾ
### �Ƽs

- $ 1\ \leq\ N\ \leq\ 10^{18} $
- $ 1\ \leq\ M\ \leq\ 10000 $

### Sample Explanation 1

$ \lfloor\ \frac{10^1}{2}\ \rfloor\ =\ 5 $ �ʤΤǡ�$ 5 $ �� $ 2 $ �Ǹ�ä����� $ 1 $ ��������ޤ���

