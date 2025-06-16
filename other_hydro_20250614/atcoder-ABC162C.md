## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc162/tasks/abc162_c

$ \displaystyle{\sum_{a=1}^{K}\sum_{b=1}^{K}\sum_{c=1}^{K}\ \gcd(a,b,c)} $ �����Ƥ���������

��������$ \gcd(a,b,c) $ �� $ a,b,c $ ����󹫼s������ޤ���

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ K $

## �����ʽ
$ \displaystyle{\sum_{a=1}^{K}\sum_{b=1}^{K}\sum_{c=1}^{K}\ \gcd(a,b,c)} $ �΂���������衣

## ��Ŀ����
��
$$\sum_{a=1}^K\sum_{b=1}^K\sum_{c=1}^Kgcd(a,b,c)$$

��ֵ��

```input1
2
```

```output1
9
```

```input2
200
```

```output2
10813692
```

## ��ʾ
### �Ƽs

- $ 1\ \leq\ K\ \leq\ 200 $
- $ K $ ������

### Sample Explanation 1

$ \gcd(1,1,1)+\gcd(1,1,2)+\gcd(1,2,1)+\gcd(1,2,2) $ $ +\gcd(2,1,1)+\gcd(2,1,2)+\gcd(2,2,1)+\gcd(2,2,2) $ $ =1+1+1+1+1+1+1+2=9 $ �Ȥʤ뤿�ᡢ�𤨤� $ 9 $ �Ǥ���

