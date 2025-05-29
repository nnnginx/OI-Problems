## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc177/tasks/abc177_e

$ N $ ��������������ޤ���$ i $ ��Ŀ������ $ A_i $ �Ǥ���

��ȫ�Ƥ� $ 1\leq\ i\ <\ j\ \leq\ N $ �ˤĤ��ơ�$ GCD(A_i,A_j)=1 $�����ɤ����ĤȤ���$ \{A_i\} $ �� pairwise coprime �Ǥ���Ȥ����ޤ���

$ \{A_i\} $ �� pairwise coprime �ǤϤʤ������ġ�$ GCD(A_1,\ldots,A_N)=1 $ �Ǥ���Ȥ���$ \{A_i\} $ �� setwise coprime �Ǥ���Ȥ����ޤ���

$ \{A_i\} $ �� pairwise coprime��setwise coprime�����Τɤ���Ǥ�ʤ����Τ�����Ǥ��뤫�ж����Ƥ���������

������ $ GCD(\ldots) $ ����󹫼s������ޤ���

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ A_1 $ $ \ldots $ $ A_N $

## �����ʽ
$ \{A_i\} $ �� pairwise coprime �ʤ�� `pairwise coprime`��setwise coprime �ʤ�� `setwise coprime`�����Τɤ���Ǥ�ʤ���� `not coprime` �ȳ������衣

## ��Ŀ����
��һ������Ϊ $N$ ������ $A$ �������������� $1 \leq i < j \leq n, gcd(A_i,A_j)=1$����� `pairwise coprime`������� $gcd(A_1,\ldots ,A_n)=1$,�����`setwize coprome`�������`not coprime`

```input1
3
3 4 5
```

```output1
pairwise coprime
```

```input2
3
6 10 15
```

```output2
setwise coprime
```

```input3
3
6 10 16
```

```output3
not coprime
```

## ��ʾ
### �Ƽs

- $ 2\ \leq\ N\ \leq\ 10^6 $
- $ 1\ \leq\ A_i\leq\ 10^6 $

### Sample Explanation 1

$ GCD(3,4)=GCD(3,5)=GCD(4,5)=1 $ �ʤΤ� pairwise coprime �Ǥ���

### Sample Explanation 2

$ GCD(6,10)=2 $ �ʤΤ� pairwise coprime �ǤϤ���ޤ��󤬡�$ GCD(6,10,15)=1 $ �ʤΤ� setwise coprime �Ǥ���

### Sample Explanation 3

$ GCD(6,10,16)=2 $ �ʤΤǡ�pairwise coprime �Ǥ� setwise coprime �Ǥ⤢��ޤ���

