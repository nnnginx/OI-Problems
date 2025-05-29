## ��Ŀ����
Farmer John is continuing to ponder the issue of cows crossing the road through his farm, introduced in the preceding two problems. He realizes now that the threshold for friendliness is a bit more subtle than he previously considered -- breeds $a$ and $b$ are now friendly if $|a - b| \leq K$, and unfriendly otherwise.
Given the orderings of fields on either side of the road through FJ's farm, please count the number of unfriendly crossing pairs of breeds, where a crossing pair of breeds is defined as in the preceding problems.



## �����ʽ
The first line of input contains $N$ ($1 \leq N \leq 100,000$) and $K$ ($0 \leq K < N$). The next $N$ lines describe the order, by breed ID, of fields on one side of the road; each breed ID is an integer in the range $1 \ldots N$. The last $N$ lines describe the order, by breed ID, of the fields on the other side of the road. Each breed ID appears exactly once in each ordering.


## �����ʽ
Please output the number of unfriendly crossing pairs of breeds.



## ��Ŀ����
### ��Ŀ����

Farmer John ����˼����ţ������ũ����·�����⣬���������ǰ�����������Ѿ����ܹ�����������ʶ�����Ѻöȵ���ֵ����֮ǰ���ǵ�Ҫ΢��һЩ�������ڣ�Ʒ�� $a$ �� $b$ ���Ѻõĵ��ҽ��� $|a - b| \leq K$��������ǲ��Ѻõġ����� FJ ũ����·������ص�Ʒ��˳������㲻�ѺõĽ���Ʒ�ֶԵ����������н���Ʒ�ֶԵĶ�����ǰ����������ͬ��

### �����ʽ

����ĵ�һ�а��� $N$ ($1 \leq N \leq 100,000$) �� $K$ ($0 \leq K < N$)���������� $N$ �������˵�·һ����ص�Ʒ��˳��ÿ��Ʒ�� ID ��һ���� $1 \ldots N$ ��Χ�ڵ����������� $N$ �������˵�·��һ����ص�Ʒ��˳��ÿ��Ʒ�� ID ��ÿ��˳����ǡ�ó���һ�Ρ�

### �����ʽ

��������ѺõĽ���Ʒ�ֶԵ�������

### ˵��/��ʾ

����������У�Ʒ�� 1 �� 4 �ǲ��Ѻõ��ҽ���ģ�Ʒ�� 1 �� 3 Ҳ�ǲ��Ѻõ��ҽ���ġ�

```input1
4 1
4
3
2
1
1
4
2
3
```

```output1
2
```

## ��ʾ
In this example, breeds 1 and 4 are unfriendly and crossing, as are breeds 1 and 3.



