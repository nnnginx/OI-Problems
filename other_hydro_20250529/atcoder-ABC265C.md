## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc265/tasks/abc265_c

�k $ H $ �ޥ����� $ W $ �ޥ��Υ���åɤ�����ޤ����Ϥ��� $ i $ ��Ŀ���󤫤� $ j $ ��Ŀ�Υޥ��� $ (i,j) $ �ȱ��ޤ���  
 $ (i,j) $ �ˤ����� $ G_{i,j} $ ���������ޤ�Ƥ��ޤ��������� $ G_{i,j} $ �� `U`, `D`, `L`, `R` �Τ����줫�Ǥ���

���ʤ��� $ (1,1) $ �ˤ��ޤ������ʤ����ƄӤ��뤳�Ȥ��Ǥ��ʤ��ʤ�ޤǴΤβ������R�귵���ޤ���

> ���ʤ��ϬF�� $ (i,j) $ �ˤ���Ȥ��롣  
>  $ G_{i,j} $ �� `U` �Ǥ��ꡢ���� $ i\ \neq\ 1 $ �ʤ�� $ (i-1,j) $ ���ƄӤ��롣  
>  $ G_{i,j} $ �� `D` �Ǥ��ꡢ���� $ i\ \neq\ H $ �ʤ�� $ (i+1,j) $ ���ƄӤ��롣  
>  $ G_{i,j} $ �� `L` �Ǥ��ꡢ���� $ j\ \neq\ 1 $ �ʤ�� $ (i,j-1) $ ���ƄӤ��롣  
>  $ G_{i,j} $ �� `R` �Ǥ��ꡢ���� $ j\ \neq\ W $ �ʤ�� $ (i,j+1) $ ���ƄӤ��롣  
>  ��������Έ��ϡ����ʤ����ƄӤ��뤳�Ȥ��Ǥ��ʤ���

������K�ˤ����r��Ǥ��ʤ�������ޥ���������Ƥ���������  
 �����������ʤ���������K�ˤ��뤳�Ȥʤ��o�ޤ��ƄӤ��A������Ϥ� `-1` ��������Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ H $ $ W $ $ G_{1,1}G_{1,2}\dots\ G_{1,W} $ $ G_{2,1}G_{2,2}\dots\ G_{2,W} $ $ \vdots $ $ G_{H,1}G_{H,2}\dots\ G_{H,W} $

## �����ʽ
������K�ˤ����r��Ǥ��ʤ��� $ (i,j) $ �ˤ�����ϤϴΤ���ʽ�ǳ������衣

> $ i $ $ j $

�ޤ����o�ޤ˄Ӥ��A������Ϥ� `-1` ��������衣

## ��Ŀ����
����һ������ $g$��������������� `LRUD` �ĸ���ĸ��

һ�������˴ӵ� $(1,1)$ ���������������˵� $(x,y)$����

��� $g_{x,y}$ �� `U`���ƶ��� $(x-1,y)$��

��� $g_{x,y}$ �� `D`���ƶ��� $(x+1,y)$��

��� $g_{x,y}$ �� `L`���ƶ��� $(x,y-1)$��

��� $g_{x,y}$ �� `R`���ƶ��� $(x,y+1)$��

���ĳһ���ƶ���С�������߳��������������������߳��ķ������С�����˲������߳��������� $-1$��

```input1
2 3
RDU
LRU
```

```output1
1 3
```

```input2
2 3
RRD
ULL
```

```output2
-1
```

```input3
9 44
RRDDDDRRRDDDRRRRRRDDDRDDDDRDDRDDDDDDRRDRRRRR
RRRDLRDRDLLLLRDRRLLLDDRDLLLRDDDLLLDRRLLLLLDD
DRDLRLDRDLRDRLDRLRDDLDDLRDRLDRLDDRLRRLRRRDRR
DDLRRDLDDLDDRLDDLDRDDRDDDDRLRRLRDDRRRLDRDRDD
RDLRRDLRDLLLLRRDLRDRRDRRRDLRDDLLLLDDDLLLLRDR
RDLLLLLRDLRDRLDDLDDRDRRDRLDRRRLDDDLDDDRDDLDR
RDLRRDLDDLRDRLRDLDDDLDDRLDRDRDLDRDLDDLRRDLRR
RDLDRRLDRLLLLDRDRLLLRDDLLLLLRDRLLLRRRRLLLDDR
RRRRDRDDRRRDDRDDDRRRDRDRDRDRRRRRRDDDRDDDDRRR
```

```output3
9 5
```

## ��ʾ
### �Ƽs

- $ 1\ \leq\ H,\ W\ \leq\ 500 $
- $ G_{i,j} $ �� `U`, `D`, `L`, `R` �Τ����줫�Ǥ��롣
- $ H,\ W $ �������Ǥ��롣

### Sample Explanation 1

���ʤ��� $ (1,\ 1)\ \to\ (1,\ 2)\ \to\ (2,\ 2)\ \to\ (2,\ 3)\ \to\ (1,\ 3) $ ��혤˄Ӥ������Ȥ˲�����K�ˤ��ޤ�����äƴ𤨤� $ (1,\ 3) $ �Ǥ���

### Sample Explanation 2

���ʤ��� $ (1,\ 1)\ \to\ (1,\ 2)\ \to\ (1,\ 3)\ \to\ (2,\ 3)\ \to\ (2,\ 2)\ \to\ (2,\ 1)\ \to\ (1,\ 1)\ \to\ (1,\ 2)\ \to\ \dots $ �Ȥ����褦�˟o�ޤ˄Ӥ��A���ޤ������Έ��Ϥ� `-1` ��������ޤ���

