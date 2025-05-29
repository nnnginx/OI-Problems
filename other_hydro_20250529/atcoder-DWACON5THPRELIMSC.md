## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/dwacon5th-prelims/tasks/dwacon5th_prelims_c

�ɥ�󥴤Υ���ƥ�����Ż��P�����ƥ� Dwango Media Cluster �ϡ��Ԥ��� DMC �Ⱥ��Ф�Ƥ��ޤ���  
 ������ǰ�򤫤ä������ȸФ����˥�󥴤���ϡ������Ф� DMC �餷���������Ȥ��ƶ��x���뤳�Ȥˤ��ޤ�����  
 ����Ĥˤϡ��L�� $ N $ �Τ��������� $ S $ ��3���Ϥ����� $ k $ ���뤨��줿�r�����¤򜺤���������3�ĽM $ (a,b,c) $ �΂����� $ S $ �� $ k $-DMC ���Ⱥ��֤��Ȥˤ��ޤ���

- $ 0\ \leq\ a $
- $ S[a] $ = `D`
- $ S[b] $ = `M`
- $ S[c] $ = `C`
- $ c-a $

�����ǡ�$ S[a] $ �� $ S $ �� $ a $ ��Ŀ�����֤���ޤ������^�����֤� $ 0 $ ����Ŀ�Ȥ��ƒQ���ޤ� (�Ĥޤꡢ$ 0\ \leq\ a\ \leq\ N\ -\ 1 $ �Ǥ�)��

���������� $ S $ �� $ Q $ �������� $ k_0,\ k_1,\ ...,\ k_{Q-1} $ �ˌ����ơ�$ k_i $-DMC ���򤽤줾��Ӌ�㤷�Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ S $ $ Q $ $ k_{0} $ $ k_{1} $ $ ... $ $ k_{Q-1} $

## �����ʽ
$ Q $ �г������衣  
 $ i $ ��Ŀ $ (0\ \leq\ i\ \leq\ Q-1) $ �ˤϡ������� $ S $ �� $ k_i $-DMC ����������衣

## ��Ŀ����
����һ���ַ������� $N$ ���ַ��� $S$ �Լ� $Q$ �β�ѯ��ÿ�θ���һ�� $k$ ֵ������ÿ�β�ѯ����������������������� $(D,M,C)$ ������

$0��a<b<c��N-1$ 
$S[a]=D��S[b]=M��S[c]=C$   
$c-a<k$

```input1
18
DWANGOMEDIACLUSTER
1
18
```

```output1
1
```

```input2
18
DDDDDDMMMMMCCCCCCC
1
18
```

```output2
210
```

```input3
54
DIALUPWIDEAREANETWORKGAMINGOPERATIONCORPORATIONLIMITED
3
20 30 40
```

```output3
0
1
2
```

```input4
30
DMCDMCDMCDMCDMCDMCDMCDMCDMCDMC
4
5 10 15 20
```

```output4
10
52
110
140
```

## ��ʾ
### �Ƽs

- $ 3\ \leq\ N\ \leq\ 10^6 $
- $ S $ ��`A` - `Z` ����ʤ�������
- $ 1\ \leq\ Q\ \leq\ 75 $
- $ 3\ \leq\ k_i\ \leq\ N $
- �����Ȥ����뤨���������Ϥ��٤������Ǥ���

### Sample Explanation 1

$ (a,b,c)\ =\ (0,\ 6,\ 11) $ �������򜺤����ޤ��� Dwango Media Cluster �ϡ��˥�󥴤���ζ��x�Ǥ������ DMC �餷���ʤ��褦�Ǥ���

### Sample Explanation 2

$ 6\times\ 5\times\ 7 $ ���νM�ߺϤ碌�����ꤨ�ޤ���

### Sample Explanation 3

$ c-a\ �����������\ (a,\ b,\ c)\ =\ (0,\ 23,\ 36),\ (8,\ 23,\ 36) $ ���������ޤ��� ���ʤߤˡ�DWANGO �ϡ�Dial-up Wide Area Network Gaming Operation�����^���֤Ǥ���

