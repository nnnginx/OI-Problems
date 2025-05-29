## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc205/tasks/abc205_c

�� $ X $ �� $ Y $ �ؒ줱����Τ�$ X $ �� $ Y $ �\���Ȥ�����$ \text{pow}(X,Y) $ �Ǳ��ޤ��� ������ $ \text{pow}(2,3)=2\times\ 2\times\ 2=8 $ �Ǥ���

$ 3 $ �Ĥ����� $ A,B,C $ ���뤨����Τǡ�$ \text{pow}(A,C) $ �� $ \text{pow}(B,C) $ �δ�С����^���Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ A $ $ B $ $ C $

## �����ʽ
$ \text{pow}(A,C)\ <\ \text{pow}(B,C) $ �ʤ� `<` ��$ \text{pow}(A,C)\ >\ \text{pow}(B,C) $ �ʤ� `>` ��$ \text{pow}(A,C)=\text{pow}(B,C) $ �ʤ� `=` ��������衣

## ��Ŀ����
### ��Ŀ����

������������ $A, B, C$ ��

�� $A^C > B^C$ �� ��� `>`��

�� $A^C < B^C$ �� ��� `<`��

�� $A^C = B^C$ �� ��� `=`��

```input1
3 2 4
```

```output1
>
```

```input2
-7 7 2
```

```output2
=
```

```input3
-8 6 3
```

```output3
<
```

## ��ʾ
### �Ƽs

- $ -10^9\ \leq\ A,B\ \leq\ 10^9 $
- $ 1\ \leq\ C\ \leq\ 10^9 $
- ������ȫ������

### Sample Explanation 1

$ \text{pow}(3,4)=81 $, $ \text{pow}(2,4)=16 $ �Ǥ���

### Sample Explanation 2

$ \text{pow}(-7,2)=49 $, $ \text{pow}(7,2)=49 $ �Ǥ���

### Sample Explanation 3

$ \text{pow}(-8,3)=-512 $, $ \text{pow}(6,3)=216 $ �Ǥ���

