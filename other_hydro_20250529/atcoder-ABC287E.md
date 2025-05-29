## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc287/tasks/abc287_e

ӢС���֤���ʤ������Ф� $ N $ ���뤨���ޤ���$ i\ \,\ (i\ =\ 1,\ 2,\ \dots,\ N) $ ��Ŀ�Τ�Τ� $ S_i $ �ȱ��ޤ���

���Ĥ������� $ x,\ y $ �ˌ��������¤�������ȫ�Ɯ������������� $ n $ �� $ \mathrm{LCP}(x,\ y) $ �ȱ��ޤ���

- $ x,\ y $ ���L���Ϥ������ $ n $ ����
- $ 1 $ ���� $ n $ ���¤�ȫ�Ƥ����� $ i $ �ˌ�����$ x $ �� $ i $ ����Ŀ�� $ y $ �� $ i $ ����Ŀ���Ȥ���
 
ȫ�Ƥ� $ i\ =\ 1,\ 2,\ \dots,\ N $ �ˌ��������¤΂������Ƥ���������

- $ \displaystyle\ \max_{i\ \neq\ j}\ \mathrm{LCP}(S_i,\ S_j) $

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## �����ʽ
$ N $ �г������衣$ i\ \,\ (i\ =\ 1,\ 2,\ \dots,\ N) $ ��Ŀ�ˤϡ�$ \displaystyle\ \max_{i\ \neq\ j}\ \mathrm{LCP}(S_i,\ S_j) $ ��������衣

## ��Ŀ����
���� $N$ ���ַ��� $S_i$�������
$$
\max_{i \ne j} \text{LCP}(S_i, S_i)
$$

���� $\text{LCP}(S_i, S_j)$ ��ʾ���ַ��������ǰ׺�ĳ��ȡ�

```input1
3
abc
abb
aac
```

```output1
2
2
1
```

```input2
11
abracadabra
bracadabra
racadabra
acadabra
cadabra
adabra
dabra
abra
bra
ra
a
```

```output2
4
3
2
1
0
1
0
4
3
2
1
```

## ��ʾ
### �Ƽs

- $ 2\ \leq\ N\ \leq\ 5\ \times\ 10^5 $
- $ N $ ������
- $ S_i $ ��ӢС���֤���ʤ��L�� $ 1 $ ���Ϥ������� $ (i\ =\ 1,\ 2,\ \dots,\ N) $
- $ S_i $ ���L���ξt�ͤ� $ 5\ \times\ 10^5 $ ����
 
### Sample Explanation 1

$ \mathrm{LCP}(S_1,\ S_2)\ =\ 2,\ \mathrm{LCP}(S_1,\ S_3)\ =\ 1,\ \mathrm{LCP}(S_2,\ S_3)\ =\ 1 $ �Ǥ���

