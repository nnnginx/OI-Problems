## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc233/tasks/abc233_b

���� $ L,R $ �ȡ�ӢС���֤Τߤ���ʤ������� $ S $ ���뤨���ޤ���  
 $ S $ �� $ L $ ����Ŀ���� $ R $ ����Ŀ�ޤǤβ��֤�ܞ����(���ʤ���� $ L $ ����Ŀ���� $ R $ ����Ŀ�ޤǤ����֤΁K�Ӥ���ˤ���)�����Ф�������Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ L $ $ R $ $ S $

## �����ʽ
���}�Ĥ�ָʾͨ��������衣

## ��Ŀ����
����һ���ַ��� $s$ ��һ������ $[l,r]$���� $s_l$ �� $s_r$ ���ַ���ת�������

��װ���� $s_l$ �ı�Ϊ $s_r$��$s_{l+1}$ �ı�Ϊ $s_{r-1}$��$\cdots$��$s_r$ �ı�Ϊ $s_l$��

Translated by ShanCreeper.

```input1
3 7
abcdefgh
```

```output1
abgfedch
```

```input2
1 7
reviver
```

```output2
reviver
```

```input3
4 13
merrychristmas
```

```output3
meramtsirhcyrs
```

## ��ʾ
### �Ƽs

- $ S $ ��ӢС���֤Τߤ���ʤ롣
- $ 1\ \le\ |S|\ \le\ 10^5 $ ($ |S| $ �� $ S $ ���L��)
- $ L,R $ ������
- $ 1\ \le\ L\ \le\ R\ \le\ |S| $

### Sample Explanation 1

`abcdefgh` �� $ 3 $ ����Ŀ���� $ 7 $ ����Ŀ�ޤǤβ��֤�ܞ����ȡ� `abgfedch` �Ȥʤ�ޤ���

### Sample Explanation 2

�������Фä��Y����Ԫ�������Ф�ͬһ�Ǥ��뤳�Ȥ⤢��ޤ���

