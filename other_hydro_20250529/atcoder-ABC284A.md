## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc284/tasks/abc284_a

$ N $ ���������� $ S_1,S_2,\ldots,S_N $ ������혷����뤨���ޤ���

$ S_N,S_{N-1},\ldots,S_1 $ ��혷��ǳ������Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## �����ʽ
$ N $ �г������衣 $ i\ (1\leq\ i\ \leq\ N) $ ��Ŀ�ˤϡ�$ S_{N+1-i} $ ��������衣

## ��Ŀ����
���� $N$ ���ַ�����$S_1,S_2 ... S_n$��

���� $N$ ���ַ�������������� $S_n,S_{n-1} ... S_1$�����м���һ�����и�����

���ݱ�֤ $ 1 \leq N \leq 10$��

translate by [ChrisWangZi](https://www.luogu.com.cn/user/637180)

```input1
3
Takahashi
Aoki
Snuke
```

```output1
Snuke
Aoki
Takahashi
```

```input2
4
2023
Year
New
Happy
```

```output2
Happy
New
Year
2023
```

## ��ʾ
### �Ƽs

- $ 1\leq\ N\ \leq\ 10 $
- $ N $ ������
- $ S_i $ ��ӢС���֡�Ӣ�����֡����֤���ʤ��L�� $ 1 $ ���� $ 10 $ ���¤�������
 
### Sample Explanation 1

$ N=3 $��$ S_1= $ `Takahashi`��$ S_2= $ `Aoki`��$ S_3= $ `Snuke` �Ǥ��� ��äơ�`Snuke`��`Aoki`��`Takahashi` ��혤ǳ������ޤ���

### Sample Explanation 2

�뤨���������Ф����֤򺬤ळ�Ȥ⤢��ޤ���

