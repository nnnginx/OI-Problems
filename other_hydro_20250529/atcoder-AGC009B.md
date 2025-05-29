��ֵ��$800$ ��

## ��Ŀ����

�� $N$ �������߲μ���һ���������ܹ������� $N-1$ ����̭����

����ĳЩԭ�򣬱������ܶ����в����߶�������ƽ����Ҳ����˵��Ϊ��Ӯ�ùھ���������еı�������������ÿ����������˵�����ǲ�ͬ�ġ���̭���Ľṹ���ڱ�������ĩβ������ʽ������

ÿ����������һ��ʤ�ߺ�һ�����ߡ����ʣ�µ���λ�����߽���Ϊ�ھ���

![](https://atcoder.jp/img/agc009/783f7be9c88350e31963edba8a958879.png)

ͼ��һ����̭��������

Ϊ�˷�������������߱����Ϊ $1$ �� $N$�����Ϊ $1$ ��ѡ���ǹھ������Ϊ $i$��$2 \leq i\leq N$����ѡ��������Ϊ $a_i$ ��ѡ�ֵı����б����ܡ�

���ǽ������ġ���ȡ�����ΪΪ��սʤ���в�����Ӯ�ùھ���������е�������������

�ҳ��������ܵ���С��ȡ�

��������ʽ�������¡��ڵ� $i$ �������У�����ѡ���е�һ���໥�Կ���

- ����Ԥ��ȷ���Ĳ����ߣ�
- һ��Ԥ��ȷ���Ĳ����ߺ͵� $j$��$j < i$��$j$ ��Ԥ��ȷ���ģ���������ʤ�ߣ�
- �� $j$ ���͵� $j$ ��������$j,k < i$��$j,k$ ��Ԥ��ȷ���ģ���ʤ�ߣ�

����һ�ֺϷ��ı����滮��ǰ�������۱��������Σ��κ��Ѿ��ڱ����б����ܵ�ѡ�ֶ�����μӱ�����

## ���ݷ�Χ

- $2 \leq N \leq 10^5$
- $1 \leq a_i \leq N$��$2 \leq i \leq N$��
- ��֤����Ϸ��������ٴ���һ�����������ı�����

## �����ʽ

���밴�����¸�ʽ�ӱ�׼���������

> $N$
> 
> $a_2$
> 
> :
> 
> $a_N$

## �����ʽ

�����������С������ȡ�

```input1
5
1
1
2
4
```

```output1
3
```

The following tournament and the result of the matches are consistent with the given information:

- In the first match, contestants $4$ and $5$ played against each other, and contestant $4$ won.
- In the second match, contestants $2$ and $4$ played against each other, and contestant $2$ won.
- In the third match, contestants $1$ and $3$ played against each other, and contestant $1$ won.
- In the fourth match, contestants $1$ and $2$ played against each other, and contestant $1$ won.

![](https://atcoder.jp/img/agc009/783f7be9c88350e31963edba8a958879.png)

The depth of this tournament is $3$, since contestant $5$ must play three matches in order to win the championship.
There is no tournament with depth $2$ or less that is consistent with the given information, thus the output should be $3$.

```input2
7
1
2
1
3
1
4
```

```output2
3
```

```input3
4
4
4
1
```

```output3
3
```