## ��Ŀ����

Farmer John's $N$ cows are lined up in a row and numbered $1 \dots N$��The cows are conducting another one of their strange protests��so each cow $i$ is holding up a sign with an integer $A_i$��

FJ knows the mob of cows will behave if they are properly grouped and thus would like to arrange the cows into one or more contiguous groups so that every cow is in exactly one group and that every group has a nonnegative sum��

Help him count the number of ways he can do this��modulo $1 \times 10^9��9$��

By way of example��if $N = 4$ and the cows' signs are $2,3,��3$��and $1$��then the following are the only four valid ways of arranging the cows��

($2$ $3$ $��3$ $1$)

($2$ $3$ $��3$) ($1$)

($2$) ($3$ $��3$ $1$)

($2$) ($3$ $��3$) ($1$)

Note that this example demonstrates the rule for counting different orders of the arrangements��

���� $n$ ���������м��ֻ��ַ��������ܸı�����λ�ã���ʹ��ÿ�������ĺʹ��ڵ��� $0$��������������� $1 \times 10^9��9$ ��������

## �����ʽ

* Line $1$��A single integer��$N$

* Lines $2 \times N + 1$��Line $i + 1$ contains a single integer��$A_i$

## �����ʽ

* Line $1$��A single integer��the number of arrangements modulo $1 \times 10^9��9$��

```input1
4
2
3
-3
1
```

```output1
4
```

## ��Ŀ��Դ

Gold

## ���ݹ�ģ��Լ��

$100\%$ ���������㣺$1 \le N \le 1 \times 10^5$��$��1 \times 10^4 \le A_i \le 1 \times 10^4$��
