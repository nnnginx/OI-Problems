## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/agc061/tasks/agc061_a

���� $ A_1,\ \ldots,\ A_N $ �����ꡢ�Ϥ���ȫ�Ƥ� $ i $ �ˤĤ��� $ A_i\ =\ i $ �Ǥ������ $ \mathrm{shuffle}(L,\ R) $ �����¤Ȥ��ƶ��x���ޤ���

- $ R\ =\ L\ +\ 1 $ �ʤ顢$ A_L $ �� $ A_R $ �΂�������椨�ƽK�ˤ��롣
- �����Ǥʤ��ʤ顢$ \mathrm{shuffle}(L,\ R\ -\ 1) $ ��g�Ф��Ƥ��� $ \mathrm{shuffle}(L\ +\ 1,\ R) $ ��g�Ф��롣

$ \mathrm{shuffle}(1,\ N) $ ���Ф��Ȥ��ޤ�����혽K����� $ A_K $ �΂���������Ƥ���������

�������ե�����ˤĤ��ơ��ƥ��ȥ��`���� $ T $ ���⤤�Ƥ���������

## �����ʽ
�����ϡ��˜������������¤���ʽ���뤨���롣

> $ T $ $ case_1 $ $ case_2 $ $ \vdots $ $ case_T $

�����`���ϡ����¤���ʽ�Ǥ��롣

> $ N $ $ K $

## �����ʽ
$ T $ �г������衣$ i $ ��Ŀ�ˡ�$ i $ ��Ŀ�Υƥ��ȥ��`���δ𤨤�������뤳�ȡ�

## ��Ŀ����
## ��Ŀ����

����һ�����г���Ϊ $n(n\le10^{18})$ ������ $A$����ʼ $A_i=i$�����ڶ�������һ�� $\mathrm{shuffle}(1,n)$ ������$\mathrm{shuffle}(L,R)$ �Ķ������£�
- $ R\ =\ L\ +\ 1 $ ʱ��$\mathrm{swap}(A_L,A_R)$
- ��������ִ�� $\mathrm{shuffle}(L,R-1)$, $\mathrm{shuffle}(L+1,R)$

����Ҫ��� $ \mathrm{shuffle}(1,\ n) $ ִ����Ϻ�$A_k (1\le k\le n)$ ��ֵ���� $T$ �����ݡ�

```input1
7
2 1
2 2
5 1
5 2
5 3
5 4
5 5
```

```output1
2
1
2
4
1
5
3
```

## ��ʾ
### �Ƽs

- $ 1\ \leq\ T\ \leq\ 1000 $
- $ 2\ \leq\ N\ \leq\ 10^{18} $
- $ 1\ \leq\ K\ \leq\ N $

### Sample Explanation 1

$ N=2 $ �ΤȤ��ϡ����¤��Фä� $ A=(2,1) $ ��äޤ��� - $ \mathrm{shuffle}(1,\ 2) $ ��g�Ф���$ A_1 $ �� $ A_2 $ ������椨�롣 $ N=5 $ �ΤȤ��ϡ����¤��Фä� $ A=(2,4,1,5,3) $ ��äޤ��� - $ \mathrm{shuffle}(1,\ 5) $ ��g�Ф��롣 - $ \mathrm{shuffle}(1,\ 4) $ ��g�Ф��롣 - $ \mathrm{shuffle}(1,\ 3) $ ��g�Ф��롣 - $ \vdots $ - $ \mathrm{shuffle}(2,\ 4) $ ��g�Ф��롣 - $ \vdots $ - $ \mathrm{shuffle}(2,\ 5) $ ��g�Ф��롣 - $ \mathrm{shuffle}(2,\ 4) $ ��g�Ф��롣 - $ \vdots $ - $ \mathrm{shuffle}(3,\ 5) $ ��g�Ф��롣 - $ \vdots $

