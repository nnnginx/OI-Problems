## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc283/tasks/abc283_f

$ (1,2,\ldots,N) $ ����� $ P=(P\ _\ 1,P\ _\ 2,\ldots,P\ _\ N) $ ���뤨���ޤ���

���٤Ƥ� $ i\ (1\leq\ i\leq\ N) $ �ˌ����ơ����¤΂������Ƥ���������

- $ D\ _\ i=\displaystyle\min_{j\neq\ i}\left\lparen\left\lvert\ P\ _\ i-P\ _\ j\right\rvert+\left\lvert\ i-j\right\rvert\right\rparen $
 
 ��ФȤ� $ (1,2,\ldots,N) $ ����ФȤϡ�$ (1,2,\ldots,N) $ ��K���椨�Ƶä������ФΤ��Ȥ򤤤��ޤ��� �Ĥޤꡢ�L�� $ N $ ������ $ A $ �� $ i\ (1\leq\ i\leq\ N) $ �������Фˤ��礦�� $ 1 $ �ؤ����F���Ȥ������Ĥ��ΤȤ����ޤ�$ (1,2,\ldots,N) $ ����ФǤ���

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ P\ _\ 1 $ $ P\ _\ 2 $ $ \ldots $ $ P\ _\ N $

## �����ʽ
$ D\ _\ i\ (1\leq\ i\leq\ N) $ �� $ i $ �ΕN혤˿հ����Ф�ǳ������衣

## ��Ŀ����
����һ�� $1 \sim n$ ������ $p = (p_1, p_2, \dots, p_n)$��

����Ҫ��ÿ�� $i$ ��� 
$$D_i = \min_{j \neq i} \left\{ \lvert p_i - p_j\rvert + \lvert i - j\rvert \right\} $$

һ�� $1\sim n$ ��������һ����Ϊ $n$ �����У����� $[1, n]$ �ڵ���������ǡ�ö������г���һ�Ρ�

$2\le n \le 2\times 10^5$��

```input1
4
3 2 4 1
```

```output1
2 2 3 3
```

```input2
7
1 2 3 4 5 6 7
```

```output2
2 2 2 2 2 2 2
```

```input3
16
12 10 7 14 8 3 11 13 2 5 6 16 4 1 15 9
```

```output3
3 3 3 5 3 4 3 3 4 2 2 4 4 4 4 7
```

## ��ʾ
### �Ƽs

- $ 2\ \leq\ N\ \leq\ 2\times10^5 $
- $ 1\ \leq\ P\ _\ i\ \leq\ N\ (1\leq\ i\leq\ N) $
- $ i\neq\ j\implies\ P\ _\ i\neq\ P\ _\ j $
- �����Ϥ��٤�����
 
### Sample Explanation 1

���Ȥ��С�$ i=1 $ �ˤĤ��� - $ j=2 $ �ΤȤ���$ \left\lvert\ P\ _\ i-P\ _\ j\right\rvert=1,\left\lvert\ i-j\right\rvert=1 $ �Ǥ��� - $ j=3 $ �ΤȤ���$ \left\lvert\ P\ _\ i-P\ _\ j\right\rvert=1,\left\lvert\ i-j\right\rvert=2 $ �Ǥ��� - $ j=4 $ �ΤȤ���$ \left\lvert\ P\ _\ i-P\ _\ j\right\rvert=2,\left\lvert\ i-j\right\rvert=3 $ �Ǥ��� ��äơ�$ j=2 $ �ΤȤ� $ \left\lvert\ P\ _\ i-P\ _\ j\right\rvert+\left\lvert\ i-j\right\rvert=2 $ ����С�Ȥʤ�Τǡ�$ D\ _\ 1=2 $ �Ǥ���

