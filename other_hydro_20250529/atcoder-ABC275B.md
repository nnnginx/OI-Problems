## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc275/tasks/abc275_b

��ؓ���� $ A,B,C,D,E,F $ �����ꡢ$ A\times\ B\times\ C\geq\ D\times\ E\times\ F $ ��ߤ����Ƥ��ޤ���  
 $ (A\times\ B\times\ C)-(D\times\ E\times\ F) $ �΂��� $ 998244353 $ �Ǹ�ä��������Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ A $ $ B $ $ C $ $ D $ $ E $ $ F $

## �����ʽ
$ (A\times\ B\times\ C)-(D\times\ E\times\ F) $ �� $ 998244353 $ �Ǹ�ä����������ǳ������衣

## ��Ŀ����
���� $A,B,C,D,E,F(0\le A,B,C,D,E,F\le10^{18})$����� $(A\times B\times C)-(D\times E \times F) \mod 998244353$

```input1
2 3 5 1 2 4
```

```output1
22
```

```input2
1 1 1000000000 0 0 0
```

```output2
1755647
```

```input3
1000000000000000000 1000000000000000000 1000000000000000000 1000000000000000000 1000000000000000000 1000000000000000000
```

```output3
0
```

## ��ʾ
### �Ƽs

- $ 0\leq\ A,B,C,D,E,F\leq\ 10^{18} $
- $ A\times\ B\times\ C\geq\ D\times\ E\times\ F $
- $ A,B,C,D,E,F $ ������

### Sample Explanation 1

$ A\times\ B\times\ C=2\times\ 3\times\ 5=30 $, $ D\times\ E\times\ F=1\times\ 2\times\ 4=8 $ ��ꡢ $ (A\times\ B\times\ C)-(D\times\ E\times\ F)=22 $ �Ǥ��ꡢ����� $ 998244353 $ �Ǹ�ä����Ǥ��� $ 22 $ ��������ޤ���

### Sample Explanation 2

$ A\times\ B\times\ C=1000000000 $, $ D\times\ E\times\ F=0 $ ��ꡢ $ (A\times\ B\times\ C)-(D\times\ E\times\ F)=1000000000 $ �Ǥ��ꡢ����� $ 998244353 $ �Ǹ�ä����Ǥ��� $ 1755647 $ ��������ޤ���

### Sample Explanation 3

$ (A\times\ B\times\ C)-(D\times\ E\times\ F)=0 $ �Ǥ��ꡢ����� $ 998244353 $ �Ǹ�ä����Ǥ��� $ 0 $ ��������ޤ���

