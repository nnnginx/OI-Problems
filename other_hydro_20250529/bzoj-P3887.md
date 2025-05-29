## ��Ŀ����

In an effort to better manage the grazing patterns of his cows, Farmer John has installed one-way cow paths all over his farm. The farm consists of $n$ fields, conveniently numbered $1...n$, with each one-way cow path connecting a pair of fields. For example, if a path connects from field $x$ to field $y$, then cows are allowed to travel from $x$ to $y$ but not from $y$ to $x$. Bessie the cow, as we all know, enjoys eating grass from as many fields as possible. She always starts in field $1$ at the beginning of the day and visits a sequence of fields, returning to field $1$ at the end of the day. She tries to maximize the number of distinct fields along her route, since she gets to eat the grass in each one (if she visits a field multiple times, she only eats the grass there once). As one might imagine, Bessie is not particularly happy about the one-way restriction on FJ's paths, since this will likely reduce the number of distinct fields she can possibly visit along her daily route. She wonders how much grass she will be able to eat if she breaks the rules and follows up to one path in the wrong direction. Please compute the maximum number of distinct fields she can visit along a route starting and ending at field $1$, where she can follow up to one path along the route in the wrong direction. Bessie can only travel backwards at most once in her journey. In particular, she cannot even take the same path backwards twice.

**���룺**

��һ������ͼ��Ȼ��ѡһ��·������յ㶼Ϊ $1$ ��·����������һ�λ��������ĳ�����淽���ߣ�������ж��ٸ�����Ա���������һ������·�������۳��ֶ����������ζԴ𰸵Ĺ��׾�Ϊ $1$��

## �����ʽ

The first line of input contains $n$ and $m$, giving the number of fields and the number of one-way paths. The following $m$ lines each describe a one-way cow path.Each line contains two distinct field numbers $x$ and $y$, corresponding to a cow path from $x$ to $y$. The same cow path will never appear more than once.

## �����ʽ

A single line indicating the maximum number of distinct fields Bessie can visit along a route starting and ending at field $1$, given that she can follow at most one path along this route in the wrong direction.

```input1
7 10
1 2
3 1
2 5
2 4
3 7
3 5
3 6
6 5
7 2
4 7
```

```output1
6
```

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$1 \le n,m \le 10^5$��

## ��Ŀ��Դ

Gold & ��л 18357