## ��Ŀ����
You are building advanced chips for machines. Making the chips is easy, but the power supply turns out to be an issue since the available batteries have varied power outputs.

Consider the problem of $n$ machines, each with two chips, where each chip is powered by $k$ batteries. Surprisingly, it does not matter how much power each chip gets, but a machine works best when its two chips have power outputs as close as possible. The power output of a chip is simply the smallest power output of its $k$ batteries.

You have a stockpile of 2nk batteries that you want to assign to the chips. It might not be possible to allocate the batteries so that in every machine both chips have equal power outputs, but you want to allocate them so that the differences are as small as possible. To be precise, you want to tell your customers that in all machines the difference of power outputs of the two chips is at most $d$, and you want to make $d$ as small as possible. To do this you must determine an optimal allocation of the batteries to the machines.

Consider Sample Input $1$. There are $2$ machines, each requiring $3$ batteries per chip, and a supply of batteries with power outputs $1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12$. You can, for instance, assign the batteries with power outputs $1, 3, 5$ to one chip, those with power $2, 4, 12$ to the other chip of the same machine, those with power $6, 8, 9$ to the third chip, and those with power $7, 10, 11$ to the fourth. The power outputs of the chips are $1, 2, 6,$ and $7$, respectively, and the difference between power outputs is $1$ in both machines. Note that there are many other ways to achieve this result.

## �����ʽ
The input consists of a single test case. A test case consists of two lines. The first line contains two positive integers: the number of machines $n$ and the number of batteries per chip $k (2nk \leq 10^6)$. The second line contains $2nk$ integers $p_i$ specifying the power outputs of the batteries $(1 \leq p_i \leq 10^9)$.

## �����ʽ
Display the smallest number $d$ such that you can allocate the batteries so that the difference of power outputs of the two chips in each machine is at most $d$.

## ��Ŀ����
**����Ŀ������**

������Ϊ���������Ƚ���оƬ������оƬ�����ף�����Դ��Ӧȴ��Ϊ��һ�����⣬��Ϊ���е�ص�������ʸ�����ͬ��

���� $n$ ̨���������⣬ÿ̨����������оƬ��ÿ��оƬ�� $k$ ���ع��硣�������ϵ��ǣ�ÿ��оƬ��õĵ������ٲ�����Ҫ��������������оƬ�Ĺ�����������ܽӽ�ʱ����Ч����ѡ�оƬ�Ĺ��������Ϊ�� $k$ ���������������С���ǿ��ص������

����һ�ѹ� $2nk$ ���أ�����Ҫ�����Ƿ������ЩоƬ�������޷�������Щ���ʹ��ÿ̨����������оƬ�Ĺ����������ȣ�����ϣ��������С����֮��Ĳ��졣������˵����ϣ�����߿ͻ������л���������оƬ�Ĺ��������������Ϊ $d$��������ϣ��ʹ $d$ ������С��Ϊ�ˣ������ȷ����ط�������������ŷ�����

������������ $1$���� $2$ ̨������ÿ��оƬ��Ҫ $3$ ���أ���һ�鹦�����Ϊ $1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12$ �ĵ�ء���������罫�������Ϊ $1, 3, 5$ �ĵ�ط����һ��оƬ�����������Ϊ $2, 4, 12$ �ĵ�ط����ͬһ��������һ��оƬ�����������Ϊ $6, 8, 9$ �ĵ�ط����������оƬ�����������Ϊ $7, 10, 11$ �ĵ�ط�������ĸ�оƬ��оƬ�Ĺ�������ֱ�Ϊ $1, 2, 6, 7$����̨�����й�������Ĳ���ֱ�Ϊ $1$��ע�⣬�������������ʽ����ʵ����һ�����

**�������ʽ��**

�������һ���������������������������С���һ�а������������������������� $n$ ��ÿ��оƬ����ĵ���� $k$ $(2nk \leq 10^6)$���ڶ��а��� $2nk$ ������ $p_i$��ָ����صĹ������ $(1 \leq p_i \leq 10^9)$��

**�������ʽ��**

���һ����С������ $d$��ʹ����Է�����Щ��أ�ʹÿ̨����������оƬ�Ĺ��������������Ϊ $d$��

���������ڣ�[ChatGPT](https://chatgpt.com/)��

```input1
2 3
1 2 3 4 5 6 7 8 9 10 11 12
```

```output1
1
```

```input2
2 2
3 1 3 3 3 3 3 3
```

```output2
2
```

