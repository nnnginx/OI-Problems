## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc155/tasks/abc155_c

$ N $ ö��ͶƱ�ü������ꡢ$ i\ (1\ \leq\ i\ \leq\ N) $ öĿ�ˤ������� $ S_i $ ��������Ƥ��ޤ���

�����줿���������त�����Ф�ȫ�ơ��Ǖ�혤�С����혤˳������Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ S_1 $ $ : $ $ S_N $

## �����ʽ
���ƤϤޤ������Ф�ȫ�ƴǕ�혤�С����혤ˡ��������Ф�ǳ������衣

## ��Ŀ����
������ $N$ ��ͶƱ�ļ��� �� $i$ ��ͶƱ $(1 \leq i \leq N)$ ����д���ַ��� $S_i$��

���ֵ�˳���ӡ�����Ʊ����¼�������ַ�����

```input1
7
beat
vet
beet
bed
vet
bet
beet
```

```output1
beet
vet
```

```input2
8
buffalo
buffalo
buffalo
buffalo
buffalo
buffalo
buffalo
buffalo
```

```output2
buffalo
```

```input3
7
bass
bass
kick
kick
bass
kick
kick
```

```output3
kick
```

```input4
4
ushi
tapu
nichia
kun
```

```output4
kun
nichia
tapu
ushi
```

## ��ʾ
### �Ƽs

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ S_i $ ��ӢС���֤Τߤ���ʤ������� $ (1\ \leq\ i\ \leq\ N) $
- $ S_i $ ���L���� $ 1 $ ���� $ 10 $ ���� $ (1\ \leq\ i\ \leq\ N) $

### Sample Explanation 1

�����줿������ `beet` �� `vet` �� $ 2 $ �ء�`beat` �� `bed` �� `bet` �� $ 1 $ �ؤǤ����������äơ�$ 2 $ �ؕ����줿 `beet` �� `vet` ��������ޤ���

