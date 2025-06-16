## ��Ŀ����
JOI-kun has $N$ go stones. The stones are numbered from $1$ to $N$. The color of each stone is an integer between $1$ and $10^9$, inclusive. In the beginning, the color of Stone $i$ ($1 \le i \le N$) is $A_i$.

From now, JOI-kun will perform $N$ operations. He will put the stones on the table in a line. The operation $i$ ($1 \le i \le N$) will be performed as follows:

1. JOI-kun will put Stone $i$ on the immediate right of Stone $i - 1$. However, when $i = 1$, JOI-kun will put Stone 1 on the table.
2. If there is a stone among Stones $1,2,\cdots,i-1$ whose current color is the same as Stone $i$, let $j$ be the maximum index of such stones, and JOI-kun will paint all of Stones $j+1,j+2,\cdots,i-1$ with the color $A_i$.

In order to confirm whether the operations are correctly performed, JOI-kun wants to know in advance the colors of the stones after all the operations are performed.

Given information of the go stones, write a program which determines the colors of the stones after the $N$ operations are performed.

## �����ʽ
Read the following data from the standard input.

> $N$  
> $A_1$  
> $A_2$  
> $\vdots$  
> $A_N$

## �����ʽ
Write $N$ lines to the standard output. The $i$-th line ($1 \le i \le N$) should contain the color of Stone $i$ after the $N$ operations are performed.

## ��Ŀ����
JOI ���� $N$ ö���ӣ����Ӵ� $1$ �� $N$ ��š�ÿ�����ӵ���ɫ�ǽ��� $1$ �� $10^9$ ֮������������� $1$ �� $10^9$��һ��ʼ���� $i$��$1 \le i \le N$��ö���ӵ���ɫ�� $A_i$��

��������JOI ����ִ�� $N$ �����������������ӷ����������ų�һ�С��� $i$��$1 \le i \le N$�����������£�

1. JOI ���Ὣ�� $i$ ö���ӷ��ڵ� $i - 1$ ö���ӵĽ��ڵ��Ҳࡣ �ر�أ��� $i = 1$ ʱ��JOI ����ֱ�ӽ��� 1 ö���ӷ��������ϡ�
2. ���ǰ $i-1$ ö������������һö���ӵ�ǰ����ɫ������ $i$ ��ͬ���� $j$ Ϊ��Щ���ӵı�ŵ����ֵ����ô JOI ����ѵ� $j+1,j+2,\cdots,i-1$ ö���ӵ���ɫ��Ϳ�� $A_i$��

Ϊ��ȷ�ϲ�����û����ȷ��ɣ�JOI ������ǰ֪�����в�����ɺ����ӵ���ɫ��

�������ӵ���Ϣ����дһ������ȷ����ִ�� $N$ �β�����ÿö���ӵ���ɫ��

```input1
6
1
2
1
2
3
2

```

```output1
1
1
1
2
2
2

```

```input2
10
1
1
2
2
1
2
2
1
1
2

```

```output2
1
1
1
1
1
1
1
1
1
2

```

## ��ʾ
## Samples

### Sample 1

The operations are performed as in the following table.

![](https://cdn.luogu.com.cn/upload/image_hosting/0newqhzt.png)

Finally, the colors of Stones 1, 2, 3, 4, 5, 6 will be 1, 1, 1, 2, 2, 2, respectively.

This sample input satisfies the constraints of Subtasks 1, 3.

### Sample 2

This sample input satisfies the constraints of all the subtasks.

## Constraints

- $1 \le N \le 2\times 10^5$.
- $1 \le A_i \le 10^9$ ($1 \le i \le N$).
- Given values are all integers.

## Subtasks

1. (25 points) $N \le 2 000$.
2. (35 points) $A_i \le 2$ ($1 \le i \le N$).
3. (40 points) No additional constraints.

