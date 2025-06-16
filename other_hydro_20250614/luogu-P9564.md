## ��Ŀ����
Dice are small, throwable objects with marked sides capable of landing in multiple positions. They are typically used to generate random values, especially in the context of tabletop games.

![](https://cdn.luogu.com.cn/upload/image_hosting/dsezqcgm.png)

The most common dice are small cubes, with faces numbered from $1$ to $6$. Number $n$ ($1 \le n \le 6$) is usually represented by a pattern of $n$ round dots, known as pips. Moreover, the pips on the $1$ and $4$ faces are colored red, while those on the $2$, $3$, $5$ and $6$ faces are black.

Little Cyan Fish has three dice. One day, he threw them onto a table, and then observed the uppermost faces. He claimed that the total number of the red pips facing up was exactly $A$, and the total number of the black pips facing up was exactly $B$.

However, you find his claim doubtful. You want to verify whether it is possible to throw three dice such that the total number of red pips facing up is $A$, and the total number of black pips facing up is $B$.

## �����ʽ
There is only one test case in each test file.

The first line of the input contains two integers $A$ and $B$ ($0 \leq A,B \leq 100$), indicating the total number of red pips facing up and the number of black pips facing up.

## �����ʽ
Output one line. If it is possible for Little Cyan Fish to throw three dice such that the total number of red pips facing up is $A$, and the total number of black pips facing up is $B$ output `Yes`. Otherwise output `No`.

## ��Ŀ����
**����Ŀ������**

���ӣ���һ�ָ�����б�ǣ��������������С�Ϳ�Ͷ�����ߣ�ͨ������������Ϸ��

![](https://cdn.luogu.com.cn/upload/image_hosting/dsezqcgm.png)

�����������һ��С�����壬ÿ�����ϱ�����˴� $1$ �� $6$ �����֡����� $n$��$1 \le n \le 6$��ͨ���� $n$ ��СԲ����ɵ�ͼ������ʾ������ $1$ ���� $4$ �����СԲ���Ǻ�ɫ�ģ��� $2$, $3$, $5$ �� $6$ �����СԲ���Ǻ�ɫ�ġ�

С������������ֻ���ӡ���һ�죬��������ֻ����Ͷ���������ϣ����۲��˳��ϵ���һ���档���������г��ϵ����У���ɫ�ĵ���֮��ǡ��Ϊ $A$������ɫ�ĵ���֮��ǡ��Ϊ $B$��

Ȼ��������С����ķ��ָе����ɡ�����Ҫȷ���Ƿ��п���Ͷ������ֻ���ӣ�ʹ�����г��ϵ����У���ɫ�ĵ���֮��ǡ��Ϊ $A$������ɫ�ĵ���֮��ǡ��Ϊ $B$��

**�������ʽ��**

ÿ�������ļ�����һ��������ݡ�

��һ�������������� $A$ �� $B$��$0 \leq A,B \leq 100$������ʾ���ϵĺ�ɫ����֮�����ɫ����֮�͡�

**�������ʽ��**

���һ�С����С�����п���Ͷ������ֻ����ʹ�����г��ϵ����У���ɫ�ĵ���֮��ǡ��Ϊ $A$������ɫ�ĵ���֮��ǡ��Ϊ $B$������� `Yes`��������� `No`��

**���������͡�**

�ڵ�һ�������У�����һ�ֺϷ��ķ���Ϊ $4, 2, 3$��

�ڵڶ��������У�����һ�ֺϷ��ķ���Ϊ $1, 1, 1$��

```input1
4 5

```

```output1
Yes

```

```input2
3 0

```

```output2
Yes

```

```input3
1 2

```

```output3
No

```

## ��ʾ
In the first example, one possible solution is $4, 2, 3$.

In the second example, one possible solution is $1, 1, 1$.

