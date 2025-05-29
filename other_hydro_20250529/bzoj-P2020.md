## ��Ŀ����

Farmer John needs to travel to town to pick up $k$ pounds of feed. Driving $D$ miles with $k$ pounds of feed in his truck costs $d \times k$ cents. The county feed lot has $n$ stores (conveniently numbered $1\ldots n$) that sell feed. Each store is located on a segment of the $x$ axis whose length is $e$. Store $i$ is at location $x_i$ on the number line and can sell FJ as much as $f_i$ pounds of feed at a cost of $c_i$ cents per pound. Amazingly, a given point on the $x$ axis might have more than one store. FJ starts at location $0$ on this number line and can drive only in the positive direction, ultimately arriving at location $e$, with at least $k$ pounds of feed. He can stop at any of the feed stores along the way and buy any amount of feed up to the the store's limit. What is the minimum amount FJ has to pay to buy and transport the $k$ pounds of feed? FJ knows there is a solution. Consider a sample where FJ needs two pounds of feed from three stores (locations: $1,3,4$) on a number line whose range is $0 \ldots 5$:

```plain
0   1   2   3   4   5
+---|---+---|---|---+
    1       1   1      Available pounds of feed
    1       2   2      Cents per pound
```

It is best for FJ to buy one pound of feed from both the second and third stores. He must pay two cents to buy each pound of feed for a total cost of $4$. When FJ travels from $3$ to $4$ he is moving $1$ unit of length and he has $1$ pound of feed so he must pay $1 \times 1 = 1$ cents. When FJ travels from $4$ to $5$ he is moving one unit and he has $2$ pounds of feed so he must pay $1 \times 2 = 2$ cents. The total cost is $4+1+2 = 7$ cents.

FJ ����ȥ�� $k$ ��ʳ�������ĳ����� $x$ ��ʳ�ÿ��һ��ͻ��� $x$ Ԫ��FJ �ĳ�����һ���ߣ��ܹ� $e$ ��·���� $e+1$ ���ط������ $0\sim 5$��FJ �� $0$ ��ʼ�ߣ��� $e$ ���������������ߣ���Ҫ�� $k$ ��ʳ������� $n$ ���̵꣬ÿ���̵��λ���� $x_i$��һ�����Ͽ����ж���̵꣩���� $f_i$ ��ʳ�ÿ�� $c_i$ Ԫ���ʵ��� $e$ ���� $k$ ��ʳ�����С���ѡ�

## �����ʽ

��һ�У�$k,e,n$��  

�ڶ��е��� $n+1$ �У�$x_i,f_i,c_i$��

## �����ʽ

û��д�������ʽ��

```input1
2 5 3
3 1 2
4 1 2
1 1 1
```
```output1
7
```

## ����˵�� 1

����ҽϽ��������̵��������һ�����ϣ�����·�ϵ�Ǯ�� $1+2=3$�����ڵ����Ǯ�� $2+2=4$��

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$1\leq k\leq 100$��$1\leq f_i\leq 100$��$1\leq n\leq100$��$1\leq e\leq350$��$0 < x_i < e$��$1\leq c_i\leq 10^6$��

## ��Ŀ��Դ

Silver